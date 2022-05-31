# gcd
to find gcd of two numbers by using cpp
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int a,b;
    cout<<"enter two numbers :"<<endl;
    cin>>a>>b;
    if(a<b)
    {
        swap(a,b);
    }
    while(b!=0)
    {
        a=a-b;
        if(a<b)
        {
            swap(a,b);
        }
    }
    cout<<"gcd of two numbers is = "<<a;
}
