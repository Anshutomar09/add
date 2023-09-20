# add

// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;
int add(int arr[], int n){
    int s;
    if(n==0){
        return 0;
    }
    if(n==1 ){
        return arr[0];
    }
    s=arr[0]+add(arr+1,n-1);
    return s;
    
}

int main() {
    int arr[5]={2,6,4,10,6};
    int sum=add(arr,5);
    cout<<sum;
    return 0;
}
