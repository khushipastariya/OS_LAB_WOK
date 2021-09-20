#include<iostream>
using namespace std;
int main()
{
	int i,n;
	float at[30],bt[30],wt[30],tat[30],temp[30],awt=0, atat=0;
	
	cout<<"Enter the number of process: ";
	cin>>n;
	cout<<"enter the burst time of the processes: ";
	for(i=0;i<n;i++)
	{
		cin>>bt[i];
	}
	cout<<"enter the arrival time of the processes: ";
	for(i=0;i<n;i++)
	{
		cin>>at[i];
	}
	cout<<"Process"<<"\t"<<"Arrival Time"<<"\t"<<"Burst Time"<<"\t"<<"Waiting time"<<"\t"<<"Turn Around Time"<<endl;
	temp[0]=0;
	for(i=0;i<n;i++)
	{
		wt[i]=0;
		tat[i]=0;
		temp[i+1]=temp[i]+bt[i];
		wt[i]=temp[i]-bt[i];
		tat[i]=wt[i]+bt[i];
		
		awt =awt + wt[i];
		atat = atat +tat[i];
		cout<<i+1<<"\t\t"<<at[i]<<"\t\t"<<bt[i]<<"\t\t"<<wt[i]<<"\t\t"<<tat[i]<<endl;
	}
	awt = awt /n ;
	cout<<"Average waiting time = "<<awt<<endl;
	atat = atat/n;
	cout<<"Average turn around time = "<<atat<<endl;
	return 0;
}
