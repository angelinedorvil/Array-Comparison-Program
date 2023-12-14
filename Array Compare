#include <stdio.h>
#include <stdlib.h>
#include <math.h>

#define SIZE 3 // how many elements the arrays will have

//Student: Angeline Dorvil


void create_arrays (int array[], int size); //function to obtain user input for array elements
void array_val (int array[], int size); // function to display value of each arrary by index
int sum_array (int array1[], int size); //function to calculate the sum of all elements in 2 arrays
void abs_val (int sum1, int sum2); //function to calculate the absolute value of the sums

int main(void)
{

printf("Comparing Arrays Project\n");

int s1[SIZE]; //creating the arrays based on the defined size
int s2[SIZE];

printf("\nEnter values for array #1:\n"); //getting user input for elements in the arrays based on the defined size
create_arrays (s1, SIZE);

array_val (s1, SIZE);

printf("\nEnter values for array #2:\n"); //cont getting user input for 2nd array
create_arrays (s2, SIZE);

array_val (s2, SIZE);

int sum_s1 = sum_array (s1, SIZE); //based on user input calculating the sum of both array
int sum_s2 = sum_array (s2, SIZE);

abs_val (sum_s1, sum_s2); //calculate the absolute value of the sums that we obtained above

 //End of the program
  return EXIT_SUCCESS;
}



void create_arrays (int array[], int size){
for (int i = 0; i<size; i++){ //number of elements input by user will be based on the size parameter
	scanf("%d", &array[i]); 	
}
}


void array_val (int array[], int size){
for (int i = 0; i<size; i++){ //displaying values by index
	printf("Value at index %d is: %d\n", i, array[i]);
}
}


int sum_array (int array[], int size){
int total = 0; // keeping track of the sum of the arrays

for (size_t i = 0; i < size; ++i) {
	total += array[i]; //add to the total by elements in each array while keeping track of the size
}
return total;
}


void abs_val (int sum1, int sum2){
int difference = 0;
if (sum1<0){  //making sure that the difference is calculated correctly if one value is a negative number
	difference = -sum1-sum2;
}else if (sum2<0){
	difference = -sum2-sum1;
}else{
	difference = sum1-sum2;
}

printf("\nThe result of my computation is: %.1f\n", fabs(difference)); //calculating the absolute value of the sum or total of all of the elements as a float
}


