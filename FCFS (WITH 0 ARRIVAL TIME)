#include<iostream>
using namespace std;
int main()
{
	int n , bt[30],wt[30],tat[30];
	float awt=0, atat=0;
	cout<<"Enter the number of processes: ";
	cin>>n;
	cout<<"Enter the burst time of processes: ";
	for(int i=0;i<n;i++)
	{
		cin>>bt[i];
	}
	cout<<"process \t burst time \t waiting time \t turn around time "<<endl;
	
	for(int i=0;i<n;i++)
	{
		wt[i]=0;
		tat[i]=0;
		for(int j=0;j<i;j++)
		{
			wt[i]=wt[i]+bt[j];
		}
		tat[i]=wt[i]+bt[i];
		awt = awt + wt[i];
		atat = atat + tat[i];
		
		cout<<i+1<<"\t\t"<<bt[i]<<"\t\t"<<wt[i]<<"\t\t"<<tat[i]<<endl;
	}
	awt = awt / n;
	cout<<"Average waiting time = "<<awt<<endl;
	atat = atat / n ;
	cout<<"Average turn around time = "<<atat;
	return 0;
}
