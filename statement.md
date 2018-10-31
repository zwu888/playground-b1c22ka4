
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
