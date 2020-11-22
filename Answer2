//Coded by Erick Augusto
//12-11-2020
#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>


typedef struct list{ int data; struct list *next; } list;

int isEmpty(const list *l){return (l==NULL);}


void swap(int *x, int *y) 
{ 

	int temp = *x; 

	*x = *y; 

	*y = temp; 
} 


void bubbleSort(int nums[], int n) 
{ 

	int i, j; 

	for (i = 0; i < n-1; i++){     
		for (j = 0; j < n-i-1; j++){

			if (nums[j] > nums[j+1]){

				swap(&nums[j], &nums[j+1]);
			}
		}
	}
} 


void printArray(int nums[], int size) 
{ 

	int i, j = 0; 

	for (i=0; i < size; i++){ 

		printf("%d ", nums[i]);

		j++;

		if(j == 5){

			printf("\n");

			j = 0;
		}
		
	}
}
	

int main(){

	int i;

	int sortedData[100];

	list* head = malloc(sizeof(list));

	head -> next = NULL;

	head -> data = rand()%100;

	sortedData[0] = head -> data;
	

	for(i = 1; i < 100; i++){
		head -> next = malloc(sizeof(list));
		head = head -> next;
		head -> data = rand()%100;
		sortedData[i] = head -> data;
	}


	bubbleSort(sortedData, 100);

	printf("Sorted data:\n");
	printArray(sortedData, 100);

	printf("\n\n");
	

	return 0;
}
