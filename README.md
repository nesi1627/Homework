# Homework
internal class Program { static void Main(string[] args)
{ //задача 1
string input = Console.ReadLine(); 
List<string>textList = input.Split(' ').ToList();
foreach (string number in textList)
{ Console.WriteLine(number); } 
//задача 2 List<int> numbers = new List<int>(); 
foreach (string item in textList) 
{ int number = int.Parse(item); numbers.Add(number); }
//задача 3 
foreach(int num in numbers)
{ Console.WriteLine(num); }
//задача 4
Console.WriteLine($"Брой на всички числа:{numbers.Count}");
//задача 5
List<int>filteredNumbers = new List<int>(); 
foreach(int num in numbers)
if(num > 0 && num % 2 == 0 && !filteredNumbers.Contains(num))
                {
                    filteredNumbers.Add(num);
                }
            }

            //задача 6
            Console.WriteLine(string.Join(",",filteredNumbers));

            //задача 7
            Console.WriteLine($"Брой на филтрираните числа:{filteredNumbers.Count}");
            Console.WriteLine($"Сума на филтрираните числа:{filteredNumbers.Sum(}");


