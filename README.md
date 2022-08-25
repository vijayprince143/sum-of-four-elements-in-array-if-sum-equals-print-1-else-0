# sum-of-four-elements-in-array-if-sum-equals-print-1-else-0
/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>

int main()
{
    int n,i,j,k,sum;
    printf("enter the size:");
    scanf("%d",&n);
    printf("enter the sum:");
    scanf("%d",&sum);
    int arr[n];
    for(i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++){
        for(j=i+1;j<n;j++){
            for(k=j+1;k<n;k++){
                if (arr[i]+arr[j]+arr[k]==sum){
                printf("1");
                return 0;
                }
                else{
                    printf("0");
                    return 0;
                }
                
            }
        }
    }
    
}
