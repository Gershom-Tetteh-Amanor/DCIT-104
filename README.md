# DCIT-104
//writing a program to calculate the average of all prime numbers from a given number to a given number
#include<iostream>
using namespace std;
int main(void)
 {
	float sum = 0.0;
	float count = 0;
	int n, n1;
	int i;
	 float avg;
	 cout<<"Enter the first term:";
	 cin>>n1;
	cout<<"Enter the number of terms:";
	cin>>n;
	
  
    for(int i=n1; i<=n; i++){
        for(int j=2; j<=i; j++){
            if(j==i){
                sum=sum+i;
                count++;
            }else if(i%j==0){
                break;
            }
        }
    }
	avg=(double) sum/count;
	cout<<"The average of all prime numbers from n1 to n  is:" << avg;	
return 0;
 }






//writing a program to calculate the average of all even numbers from 1 to a given number
#include<iostream>
using namespace std;
int main(void)
{
	float sum = 0.0;
	float count = 0;
	int n;
	 float avg;
	cout<<"Enter the number of terms:";
	cin>>n;
	float num [n];
	for(int i=1; i<=n; i++)
	if(i%2==0.0){
		sum=sum+i;
		count++;
	}
	avg=(double) sum/count;
	cout<<"The average of all even numbers from 1 to n  is:" <<  avg;
	return 0;
}
