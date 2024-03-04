//Stuffing
//Imran_gub_221Batch
#include <stdio.h>
#include <string.h>
void bitStuffing(char arr[], char brr[])
{
    int i,j;
    int cnt = 0;
    int len = strlen(arr);
    
    for(i=0, j=0; i<len; i++, j++)
    {
        brr[j]=arr[i];
        if(arr[i] =='0')
        {
           cnt++;
        }
        if(cnt == 5)
        {
            j++;
            brr[j]='1';
            cnt = 0;
        }
        if(arr[i] =='1')
        {
           cnt++;
        }
        if(cnt == 5)
        {
            j++;
            brr[j]='0';
            cnt = 0;
        }
    }
    
    brr[j] = '\0';
    len= strlen(brr);
    for( i=0; i<len; i++)
    
    printf("%c", brr[i]);
    printf("\n");
}
int main()
{
    char sig[100];
    char bitsig[100];
    printf("Input Signal: ");
    scanf("%s", sig);
    printf("Stuffed Bitstream: ");
    bitStuffing(sig, bitsig);
    
    return 0;
}
