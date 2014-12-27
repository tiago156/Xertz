Xertz
=====

## Examples

#### Hello world
Xertz
```c++
import "stdio.h"

int main:
    printf("Hello World!)
```
C++
```c++    
#include "stdio.h"

int main {
    printf("Hello World!);
}
```

#### Import
Xertz
```c++
import "stdio.h"
import "iostream"

from std import *
from std import cout, cin
```
C++
```c++
#include "stdio.h"
#include "iostream"

using namespace std;
using std::cout;
using std::cin;
```
#### Multiple line string
Xertz
```c++
string a = """
this
is
multiline
"""
string b """multiline
    string"""
```
C++
```c++
#include "string"

std::string a = "\nthis\nis\nmultiline\n";
std::string b = """multiline\n    string";
```
#### Arrays
Xertz
```c++
int a[3]
int b[6] = [
    1, 2, 3, 
    4, 5, 6
]
int c[3,2] = [[1,2],[3,4],[5,6]]
````
C++
```c++
int a[3];
int b[6] = {1, 2, 3, 4, 5, 6};
int b[3][2] = {{1,2},{3,4},{5,6}};
```

#### Enum
Xertz
```c++
enum Color:
    Red = 1
    Blue = 2
    Black = 3
    
enum Coord: 
    X = 'x'
    Y = 'y'
    Z = 'z'
    
enum Options:
    Option1
    Option2
    Option3
````
C++
```c++
enum Color {
    Red = 1,
    Blue = 2,
    Black = 3
};

enum Coord {
    X = 'x',
    Y = 'y',
    Z = 'z'
};

enum Options {
    Option1,
    Option2,
    Option3
};
```

#### Class
Xertz
```c++
@public
class Animal:
    ctor:
        pass
    @public
    int age;
    @public
    string name;
    int internal;
    
@public
class Person:
    public:
        ctor:
            pass
        int age;
        string name;
    private:
        int internal;
        
@public
class Employee(Person):

````
C++
```c++
#define pass (void)0

public class Person {
    public Person() {
        pass;
    }
    public int age;
    public string name;
}
```

#### Typedef
Xertz
```c++
type u_int = uint
````
C++
```c++
using u_int = unsigned int;
```

#### Fundamental Types
Xertz|C++
---|---
oi|df

#### Pointers
Xertz
```c++
int ptr(a) = None
int ptr(p) = addrptr(a)
valptr(p).x = 3
````
C++
```c++
int *a = nullptr;
int *p = &a;
p->x = 3;

```

#### Null
Xertz
```c++
int *p = None
````
C++
```c++
int *p = nullptr;
```


```c++
import "iostream"

from std import *

int main:
   float a, b, result
   char operation
 
   # Get numbers and mathematical operator from user input
   cin >> a >> operation >> b

   # Character constants are enclosed in single quotes
   switch operation:
       case '+':
             result = a + b
             break
       case '-':
             result = a - b
             break
       case '*':
             result = a * b
             break
       case '/':
             result = a / b
             break
       else:
             cout << "Invalid operation. Program terminated." << endl
             return -1

   # Output result
   cout << result << endl
   return 0
```

```c++
#include <iostream>
using namespace std;

int main()
{
   float a, b, result;
   char operation;
 
   // Get numbers and mathematical operator from user input
   cin >> a >> operation >> b;

   // Character constants are enclosed in single quotes
   switch(operation)
   {
   case '+':
         result = a + b;
         break;

   case '-':
         result = a - b;
         break;

   case '*':
         result = a * b;
         break;

   case '/':
         result = a / b;
         break;

   default:
         cout << "Invalid operation. Program terminated." << endl;
         return -1;
   }

   // Output result
   cout << result << endl;
   return 0;
}
```
