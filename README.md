# Insertion_in_array_with_c
INSERTION OF AN ELEMENT IN AN ARRAY(DSA)
#include<stdio.h>

int main()
{
	int po,i,n;
	printf("Enter the Size of the Array: ");
	scanf("%d",&n);
	int a[n];
	printf("Enter The Value: \n");
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	printf("Enter The position where you want to add The element:  ");
	scanf("%d",&po);
	for(i=0;i<n;i++){
		if (po==i){
			for(i=po;i<n;i++)
			{
				a[i+1]=a[i];
			}
		}
	}
	scanf("%d",&a[po]);
	for(i=0;i<n;i++)
	{
		printf("\nArray position: %d and value: %d",i,a[i]);
;	}
}
