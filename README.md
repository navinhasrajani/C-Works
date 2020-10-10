#include <iostream>
//#include<fstream>
using namespace std;
const int n=5;
template<class t>
void Min_array(t *a)
{

    t min=0;

    for(int i=0;i<n;i++)
    {
        min=a[1];
        min = a[i] < min ? a[i]: min;
    };
    //cout <<"Hello Wold\n";
    cout << "The minimum digit of given matrix is: "<< min;
}
int main()
{
    cout<<"The limit of matrix is 5\n\n";
    int amm[n];
    cout << "Enter values of matrix\n";
    for(int i=0;i<n;i++)
    {
        cout << "Value of element " << i+1 << " is: ";
        cin >> amm[i];
    };

    cout << "Your matrix is: \n";
    for(int i=0;i<n;i++)
    {
        cout << "["<< amm[i] << "]\n";
    };
    Min_array(amm);
}
