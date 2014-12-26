Xertz
=====

```c++
import "stdio.h"

int main:
    printf("Hello World!)
```

```c++    
#include "stdio.h"

int main {
    printf("Hello World!);
}
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
