# maopaopaixu
#include<stdio.h>
#include<string.h>
#include<stdlib.h>
int main(){
    int a[3][4];
    for(int i=0;i<3;i++){
        for(int j=0;j<4;j++){
            scanf("%d",&a[i][j]);
        }
    }
    int flag=1;
    for(int i=0;i<3 && flag;i++){
        for(int j=0;j<4;j++){
            if(a[i][j]<0){
               printf("%d %d %d\n",i,j,a[i][j]);
               flag=0;
               break;
            }
        }
    }
    return 0;
}
