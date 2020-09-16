# Tontun
#include <stdio.h>
int main() {
    int arr[3],i,sum = 0;
    int min,max;
    printf(" *** Display Summation ***\n");
    printf("Enter 2 whole number : ");
    //////////////////////////////
    for(i=0; i<2; i++){
        scanf("%d", &arr[i]);
}
    printf("Summation = ");
    //////////////////////////////
    max = arr[0];
    min = arr[0];
    for(i=0; i<2; i++){
       if(arr[i] > max)
        {
            max = arr[i];
        }
        if(arr[i] < min)
        {
            min = arr[i];
        }
    }
    for(i = min ; i <= max ; i++){
        sum += i ;
        if(i != max)
        {
        printf("%d + ",i);
        }
        else if (i == max)
        {
        printf("%d = %d",i,sum);
        }
        }    
    return 0 ;
}
