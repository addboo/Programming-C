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

### Ασκήσεις
1. Να δημιουργηθεί function πολλαπλασιασμού mult() η οποία όταν δέχεται έναν αριθμό, να υπολογίζει την αντίστοιχη προπαίδεια π.χ. mult(5), να εμφανίζει την προπαίδεια του 5.

```cpp
// mult_func.cpp

#include <stdio.h>
 
int mult ( int x, int y );
 
int main()
{
    mult(5);
    getchar(); 
}
 
int mult (int x)
{
    for(int k=1; k<=10; k++)
    {
        printf("%d x %d = %d \n", k, x, k*x);
    }
}
```

2. Συνεχίζοντας την προηγούμενη άσκηση, να δημιουργηθεί πρόγραμμα που να τυπώνει την προπαίδεια απο το 1 εως το 10 χρησιμοποιώντας την function mult().

```cpp
// mult_func_10.cpp

#include <stdio.h>
 
int mult (int x);
 
int main()
{
    for(int j=1; j<=10; j++)
    {
        mult(j);
        printf("\n");
    }
        
    getchar(); 
}
 
int mult (int x)
{
    for(int k=1; k<=10; k++)
    {
        printf("%d x %d = %d \n", k, x, k*x);
    }
}
```
