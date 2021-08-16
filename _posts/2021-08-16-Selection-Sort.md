---
layout: post
---

This code below is a function of Selection Sort

By finding minmimum element in unsorted array selection sort algorithms sorts the array. Also they keep track of sorted part of array and unsorted array.

Example

input = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

this input array became [1, 9, 8, 7, 6, 5, 4, 3, 2, 10] in first iteration
this input array became [1, 2, 8, 7, 6, 5, 4, 3, 9, 10] in second iteration and so on


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