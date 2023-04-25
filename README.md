# Linq-Method
## Aggregate Operators (Use To Get Number)
- SUM: The SUM operator can be used to calculate the sum of a collection of numbers
- AVG: The AVG operator can be used to find the average value of a collection of numbers
- MIN: The MIN operator can be used to find the minimum value in a collection
- MAX: The MAX operator can be used to find the maximum value in a collection
- COUNT: The COUNT operator can be used to count the number of elements in a collection

## Restriction Operator (Use To Filter Data)
``` c#
  // Where Return True Or False Depend condition You Specific
  List<Student> students = new List<Student>
  {
      new Student { Name = "Alice", Age = 14, Grade = 9 },
      new Student { Name = "Bob", Age = 16, Grade = 11 },
      new Student { Name = "Charlie", Age = 15, Grade = 10 },
      new Student { Name = "David", Age = 14, Grade = 9 },
      new Student { Name = "Emily", Age = 17, Grade = 12 }
  };
  var grade9Students = students.Where(s => s.Grade == 9);
  
  // if return true will return object else will not return any thing
     public static bool check(int data)
      {
         return data.Grade == 9;
      }
```

##  projection operator (Use To Map Data)
``` c# 
List<Student> students = new List<Student>
{
    new Student { Name = "Alice", Age = 14, Grade = 9 },
    new Student { Name = "Bob", Age = 16, Grade = 11 },
    new Student { Name = "Charlie", Age = 15, Grade = 10 },
    new Student { Name = "David", Age = 14, Grade = 9 },
    new Student { Name = "Emily", Age = 17, Grade = 12 }
};
var studentNames = students.Select(s => s.Name);
```
## ordering operator (Use To Sort Data)
- OrderBy use to order data asc
- OrderByDescending use to order data desc
- ThenBy use after use orderby when you can multi order on asc
- ThenByDescending use orderby when you can multi order on desc


## Partitioning operators in (Use Limit And Offset )
- Take Work Same Like limit 
- Skip work same like offset 


## Query execution (First Element)
``` c# 
// Use To Return Object From Array Object Or Null If Not Have Any Element
var firstEven = numbers.Where(n => n % 2 == 0).FirstOrDefault();
```
## element operator (Use Like FindIndexOf)
``` c#
List<int> numbers = new List<int> { 1, 2, 3, 4, 5 };
int thirdNumber = numbers.ElementAt(2);

```
## set operators  (Use Like SET)
- Distinct: Returns the unique elements from a collection.
- Intersect: Returns the common elements from two collections.

## generation operators  (Repeat And Empty)
- Empty: Returns an empty collection.
- Repeat: Generates a sequence that contains one repeated value.
## Concat Operator (Concat Two Element)
``` c# 
var collection1 = new List<int> { 1, 2, 3 };
var collection2 = new List<int> { 4, 5, 6 };
var collection3 = new List<int> { 7, 8, 9 };
var concat = collection1.Concat(collection2).Concat(collection3);
```

## quantifiers operators (Use Some Or Every )
- Any: Returns a Boolean value that indicates whether any elements in the sequence satisfy a given condition.
- All: Returns a Boolean value that indicates whether all elements in the sequence satisfy a given condition.
