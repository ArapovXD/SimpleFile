//Arapov Denis
#include <iostream>
#include <fstream>

using namespace std;

int main(int argc, char *argv[])
{

    int a;

    ifstream f1(argv[1]);
    ofstream f2("OData.txt");

    while (f1 >> a) f2 << (a > 0? a: 0) << " ";

    f1.close();
    f2.close();

    return 0;
}