#include<iostream>
#define many long long

int nu[100];

many fib(int n)
{
  if(n==1)  return 1;
  if(n==0)  return 0;
  if(nu[n]==0)  return fib(n-1)+fib(n-2);
  return nu[n];
}

int main(void)
{
  int n;  std::cin>>n;
  std::cout<<fib(n);
}
