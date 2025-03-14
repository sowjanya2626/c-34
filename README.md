# c-34
Indirect Recursion 
#include<stdio.h>
int one(int n){
    if(n>0){
        printf("%d",n);
        two(n-1);
    }
}
int two(int n){
    if(n>0){
            printf("%d",n);
            one(n-1);
        }
    }
    int main(){
        one(10);
        return 0;
    }
