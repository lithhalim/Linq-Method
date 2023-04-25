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


