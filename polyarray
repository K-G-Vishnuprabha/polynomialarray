#include<stdio.h>
struct term
{
    int coeff;
    int expo;
};
int main()
{
    int n1,n2,i,j,k;
    struct term p1[20],p2[20],res[20];
    printf("Enter no:of terms ");
    scanf("%d",&n1);
    for(i=0;i<n1;i++)
    {
        printf("Enter coef ");
        scanf("%d",&p1[i].coeff);
        printf("Enter expo: ");
        scanf("%d",&p1[i].expo);
    }
     printf("Enter no:of terms of 2nd ");
    scanf("%d",&n2);
    for(i=0;i<n2;i++)
    {
        printf("Enter coef ");
        scanf("%d",&p2[i].coeff);
        printf("Enter expo: ");
        scanf("%d",&p2[i].expo);
    }
    printf("\n1st polynomial:\n");
     for(i=0;i<n1;i++)
     {
        printf(" %dx^%d ",p1[i].coeff,p1[i].expo);
        if(i!=n1-1)
       {
        printf("+ ");
       }
     }
     printf("\n2nd polynomial:\n");
     for(i=0;i<n2;i++)
     {
        printf(" %dx^%d ",p2[i].coeff,p2[i].expo);
        if(i!=n2-1)
        {
        printf("+ ");
        }
     }
     i=j=k=0;
     while(i<n1&&j<n2)
     {
        if(p1[i].expo==p2[j].expo)
        {
            res[k].coeff=p1[i].coeff+p2[j].coeff;
            res[k].expo=p1[i].expo;
            i++,j++,k++;
        }
        else if(p1[i].expo>p2[j].expo)
        {
           res[k]=p1[i];
           i++,k++;
        }
        else
        {
            res[k]=p2[j];
            j++,k++;
        }
     }
     while(i<n1)
     {
        res[k]=p1[i];
        i++,k++;
     }
      while(j<n2)
     {
        res[k]=p2[j];
        j++,k++;
     }
     printf("\n Sum is:\n");
     for(i=0;i<k;i++)
     {
     printf("%dx^%d  ",res[i].coeff,res[i].expo);
     if(i!=k-1)
     {
        printf("+ ");
     }
     }
     return 0;
}
