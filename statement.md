#description: 
 This is called koenig lookup or argument dependent name lookup. In this case, the namespace 'standards' is searched for a function 'foo' because its argument 'ds' is defined in that namespace.  For function 'bar', no additional namespaces are searched and the name is not found.  More details are in 3.4.2.
```C++ runnable
#include <iostream>

namespace standards
{
    struct datastructure
    {
    };

    void foo(const datastructure& ds)
    {
    }

    void bar()
    {
    }
}

int main(int argc, char** argv)
{
    standards::datastructure ds;

    foo(ds);

    bar();

    return 0;
}
