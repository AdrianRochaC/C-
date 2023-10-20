#include <iostream>

using namespace std;

int main()
{
	int r = 0;
    int i = 0;
    int j = 0;
    int k = 0;
    int a[5];
    int b[5];
    int c[6];
    
    for(i = 0; i <= 4; i++){
    cout<<"Ingrese numero primer grupo: ";
    cin >> a[i];
    }
    
    for(j = 0; j <= 4; j++){
    cout<<"Ingrese numero segundo grupo: ";
    cin>>b[j];
    }
    
    for(k = 0; k <= 5; k++){
    	c[k] = 0;
	}
	k=0;
	for(i = 0; i <= 4; i++){
		r = a[i] % 2;
		if(r == 0){
			if(k < 3){
			c[k] = a[i];
			k++;
		}
		}
	}
	k=3;
	for(j = 0; j <= 4; j++){
		r = b[j] % 2;
		if(r == 1){
			if(k < 6){
			c[k] = b[j];
			k++;
		}
		}
	}
	cout<<"\n"; 
	cout<<"\n"; 
	for ( i = 0; i <= 4; i++){
		cout<<a[i]<<" ";
	}
	
	cout<<"\n"; 
	cout<<"\n"; 
	for (j = 0; j <= 4; j++){
		cout<<b[j]<<" ";
	}
	
	cout<<"\n";
	cout<<"\n"; 
	for (k = 0; k <= 5; k++){
		cout<<c[k]<<" ";
	}
	
    return 0;
}
