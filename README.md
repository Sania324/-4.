//Вариант3 базовый уровень .В заданной строке вместо первого символа поставить пробел,а вместо последнего-точку
#include <iostream>

using namespace std;

int main()
{
    char str[80] = "i love mother";
    char token[80];

    cout << str << endl;

    const char *p = str;
    char *t = token;
    *t++ = ( *p ? ' ' : *p ); 

    while ( *p++ )
    {
        *t++ = *p;
    }; 

    cout << token << endl;
}
