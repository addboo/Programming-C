# Συναρτήσεις
Στο παράδειγμα αυτό χρησιμοποιούμε την βιβλιοθήκη `stdio.h` σε αντίθεση με τα προηγούμενα μαθήματα που χρησιμοποιούσαμε την βιβλιοθήκη `iostream.h`. Στην `iostream` για να τυπώσουμε ένα μήνυμα στην οθόνη χρησιμοποιούσαμε την εντολή `cout`. Ενώ στην `stdio` την εντολή `printf`.

```cpp
#include <stdio.h>
 
int mult ( int x, int y );
 
int main()
{
  int x;
  int y;
   
  printf( "Please input two numbers to be multiplied: " );
  scanf( "%d", &x );
  scanf( "%d", &y );
  printf( "The product of your two numbers is %d\n", mult( x, y ) );
  getchar(); 
}
 
int mult (int x, int y)
{
  return x * y;
}
```
