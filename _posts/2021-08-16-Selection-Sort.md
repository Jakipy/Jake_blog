---
layout: post
---

This code below is a function of Selection Sort

Explaination of the function

1. Set a min value to very large number like 9999 and every time they find a value less then value of min they update min with new value 

2. Swap the min value to the first number to put small number on left and increase sorted part of array

3. keep doing number 1 and 2 in unsorted part of array



Example

input = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

this input array became [1, 9, 8, 7, 6, 5, 4, 3, 2, 10] in first iteration

this input array became [1, 2,(sorted part)|||(unsorted part) 8, 7, 6, 5, 4, 3, 9, 10] in second iteration and so on

eventually final output will be [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] which is sorted array

Pros and Cons of Selection Sort algorithm

1. Easy to under stand

2. Easy to implement

3. Not a efficent algorithm because it has time complexity of O(N^2)


{% highlight ruby %}
void selection_sort(){
	int i,j, min,index,temp;
	for(i = 0; i<n; i++){
		min = 9999;
		for(j = i; j<n;j++){
			if(min > arr[j]){
				min = arr[j];
				index = j;
			}
			
			
		}
		temp = arr[i];
		arr[i] = arr[index];
		arr[index] = temp;
	}

	
}

{% endhighlight %}


