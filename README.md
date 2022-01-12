# Class Template Specialization - Because I'm Bored

```cpp
#include <iostream>
using namespace std ;

template <class T>
class stream
{
	public:
		void f() { cout << "stream<T>::f()"<< endl ;}
} ;

template <>
class stream<char>
{
	public:
		void f() { cout << "stream<char>::f()"<< endl ;}
} ;

int main()
{
	stream<int> si ;
	stream<char> sc ;

	si.f() ;
	sc.f() ;
	
	return 0 ;
}
```
