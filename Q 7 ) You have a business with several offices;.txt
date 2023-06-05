#include<iostream>
using namespace std;

int main(){
    int a[3][3],b[3][3],c[3][3],result[3][3];
    
    cout<<"Enter A : ";
    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            cin>>a[i][j];
        }
    }

    cout<<" B ";
    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            cin>>b[i][j];
        }
    }

    cout<<" C :";
    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            cin>>c[i][j];
        }
    }

    // Checking the Matrix 
    // A and B 
    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            if(a[i][j]<b[i][j]){
                result[i][j] = a[i][j];
            }else{
                result[i][j] = b[i][j];
            }
        }
    }

    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            if(result[i][j]>c[i][j]){
                result[i][j] = c[i][j];
            }else{
                result[i][j];
            }
        }
    }

    // Printing 
    for(int i=0; i<3; i++){
        for(int j=0; j<3; j++){
            cout<<result[i][j]<<" ";
        }
    }

    return 0;
}