#include<iostream>
using namespace std;

int main()
{
    int n,r,sum=0,a=0,b=0,y,x,w=0,v,f;
    cout<<"Enter more than 3 digit number";
    cin>>n;
    int user;
    int d=n;
    cout<<"1.Find sum of number\n"
    "2.Find even and odd number\n"
    "3.Find largest number\n"
    "4.Find reverse number\n"
    "5.Find sum of odd and even"
    ;
    cout<<"\n";
    cin >> user;
    int temp=n;
    int p=n;
    int t=n;
    int o=n;
    int j,add=0,po,addi;
    
    switch(user) {
    case 1:
     while(n>0) {
     r=n%10;
      sum=sum+r;
      n=n/10;
     }
     cout<<"The sum of number :"<<sum;
     break;
     case 2:
     while(temp>0) {
     y=temp%10;
     if(temp%2==0) 
     a++;
     else 
     b++;
     temp=temp/10;
     }
     cout<<"Even number :" <<a <<endl;
     cout<<"odd number:"<< b;
     break;
     case 3:
     while(p>0) {
     x=p%10;
     if (x>w) {
     w=x;
     }
     p=p/10;
     }
     cout<<"The largest number: " <<w;
     break;
     case 4:
     while(d>0) {
     v=d%10;
     f=v;
     d=d/10;
     
     cout<<f;
     }
     break ;
     case 5:
     while (o>0) {
     po=o%10;
     if(po%2==0) 
     add=add+po;
     
     else 
     addi=addi+po;
     o=o/10;
     }
     cout<<"The addition of even number is: "<<add;
     cout<<"The addition of odd number is: "<<addi;
     
     break;
     default:
     cout<<"Bhai 1 aur 5 ke bich me daal number";
     }
     return 0;
}