# Sorting_Techinques

#include<stdio.h>
#include<stdbool.h>
#include<string.h>
#include<limits.h>
/*
// Sorting 

// Q2 . 2 - pointer question(To find the vaue by the sum of two numbers)

int main(){
	int target = 8;
	int arr[8] = {1,2,3,4,6,8,9,10};
	int n=8;
	int i = 0;
	int j = n-1;
	while(i<j){
		if(arr[i]+arr[j] == target){
			printf("Found");
			break;
		}
		else if(arr[i]+arr[j]>target){
			j--;
		}
		else i++;
	}
	return 0;
}


// Bubble Sort -- to make it in ascending order

int main(){
	int arr[5] = {5,4,3,2,1 };
	int n=5;
	for(int i=0;i<5;i++){
		printf("%d ",arr[i]);
	}
	//bubble sort
	for(int i=0;i<n-1;i++){
		bool flag = true;// array isn't sorted yet
		for(int j=0;j<=n-2;j++){
			if(arr[j]>arr[j+1]){
				int temp = arr[j];
				arr[j] = arr[j+1];
				arr[j+1] = temp;
				flag=false;
			}
		}
		if(flag == true) break;
	}
	printf("\n");
	for(int i=0;i<5;i++){
		printf("%d ",arr[i]);
	}
	return 0;
}


// Bubble Sort -- To make the order in descending
int main(){
	int arr[5] = {1,3,4,5,2};
	int n=5;
	for(int i=0;i<5;i++){
		printf("%d ",arr[i]);
	}
	//bubble sort
	for(int i=0;i<n-1;i++){
		bool flag = true;// array isn't sorted yet
		for(int j=0;j<=n-2;j++){
			if(arr[j]<arr[j+1]){
				int temp = arr[j+1];
				arr[j+1] = arr[j];
				arr[j] = temp;
				flag=false;
			}
		}
		if(flag == true) break;
	}
	printf("\n");
	for(int i=0;i<5;i++){
		printf("%d ",arr[i]);
	}
	return 0;
}


// Selection Sort 

int main(){
	int arr[7] = {7,4,5,9,8,2,1};
	int n=7;
	printf("Unsorted Array: \n");
	for(int i=0;i<n;i++){
		printf("%d ",arr[i]);
	}
	
	//selection sort
	for(int i=0;i<n-1;i++){ //n-1 passes
	int min = INT_MAX;
	int minidx = -1;
		for(int j=i;j<=n-1;j++){
			if(min>arr[j]) {
				min = arr[j];
				minidx = j;
			}
		}
		// swap the min and first element of umsorted part
		// swap minidx and i
		int temp = arr[minidx];
		arr[minidx] = arr[i];
		arr[i] = temp;
}
	printf("\n");
	printf("Sorted Array : \n");
	for(int i=0;i<n;i++){
		printf("%d ",arr[i]);
	}

	return 0;

}


// Insertion Sort

int main(){
	int arr[7] = {7,4,5,9,8,2,1};
	int n=7;
	printf("Unsorted Array: \n");
	for(int i=0;i<n;i++){
		printf("%d ",arr[i]);
	}
	// Insertion Sort	
	for(int i=1;i<=n-1;i++){
		int j = i;
		while(j>=1 && arr[j]<arr[j-1]){
			int temp = arr[j];
			arr[j] = arr[j-1];
			arr[j-1] = temp;
			j--;
		}
	}
	printf("\n");
	printf("Sorted Array : \n");
	for(int i=0;i<n;i++){
		printf("%d ",arr[i]);
	}
	return 0;
}


// Q1.Pushing the zeros in the array to the end with a copy of array

int main(){
	int arr[9] = {5,0,2,0,0,4,1,3,0};
	int ans[9];
	int idx = 0;
	for(int i=0;i<9;i++){
		if(arr[i]!=0){
			ans[idx] = arr[i];
			idx++;
		}
	}
	while(idx!=9){
		ans[idx] = 0;
		idx++;
	}
	printf("\n");
	printf("Sorted Array : \n");
	for(int i=0;i<9;i++){
		printf("%d ",ans[i]);
	}
	return 0;
}
*/

// Q2.Pushing the zeros in the array to the end without any extra array

int main(){
	int arr[9] = {5,0,2,0,0,4,1,3,0};
	int n = 9;
	printf("Unsorted Array: \n");
	for(int i=0;i<n;i++){
		printf("%d ",arr[i]);
	}
	for(int i=0;i<n-1;i++){
		bool flag = true;// array isn't sorted yet
		for(int j=0;j<=n-1-i;j++){
			if(arr[j]<arr[j+1]){
				int temp = arr[j+1];
				arr[j+1] = arr[j];
				arr[j] = temp;
				flag=false;
			}
		}
		if(flag == true) break;
	}
	printf("\n");
	printf("Sorted Array : \n");
	for(int i=0;i<9;i++){
		printf("%d ",arr[i]);
	}
	return 0;
}

//Q3. given an array of digits (values are from 0 to 9),task is to find the minimum possible sum of two numbers formed from digits of array.
// Please note that all digits of the given array must be used to form two numbers)

int main(){
	
	return 0;
}
