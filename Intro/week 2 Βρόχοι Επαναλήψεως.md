# Βρόχοι Επανάληψης for, while, do..while


```cpp
// counter_while.cpp

#include <iostream>

using namespace std;

int main() 
{
    int x = 1;

    while(x <= 10)
    {
        cout << "Epanalipsi: " << x << endl;
        x++;
    }

    system("pause");
    return 0;
}
```



### Άσκηση
Χρησιμιποιώντας την while να κατασκευάσετε πρόγραμμα που να μετράει αντίστροφα από το 10 εως το 1.

```cpp
//countdown_while.cpp

#include <iostream>

using namespace std;

int main() 
{
    int x = 10;

    while(x >= 1)
    {
        cout << "Epanalipsi: " << x << endl;
        x--;
    }

    system("pause");
    return 0;
}
```
