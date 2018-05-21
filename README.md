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
