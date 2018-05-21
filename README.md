#include <iostream>
using namespace std;

int main(){
	
	int i, j, data[50], tmp, n,pil;
	
	cout<<"Masukkan banyak data : ";
	cin>>n;
	
	for(i=1;i<=n;i++){
		cout<<"masukkan data ke-"<<i<<" : ";
		cin>>data[i];
	}
	
	cout<<"Masukkan pilihan (1/2) : \n 1. Selection sort\n 2. Bubble sort\nPilihan anda : ";
	cin>>pil;
	
	switch(pil){
		case 1 :cout<<"\nAscending :";
				for(i=1;i<=n;i++){
					for(j=1+i;j<=n;j++){
						if(data[i]>data[j]){
							tmp=data[i];
							data[i]=data[j];
							data[j]=tmp;	
						}
					}
				}
		case 2 :cout<<"\nAscending :";
				for(i=n-1;i>=1;i--){
					for(j=1;j<=i;j++){
						if(data[j]>data[j+1]){
							tmp=data[j+1];
							data[j+1]=data[j];
							data[j]=tmp;
						}
					}
				}	
	}
	
	cout<<"\nAscending :";	
	for(i=1;i<=n;i++){
		cout<<data[i]<<"  ";
	}
	
	
	return 0;
}
