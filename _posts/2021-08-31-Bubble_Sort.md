---
layout: post
---
I personally think bubble sort is easist algorithms to understand and implement.

Because it's such a easy sorting algorithms, they have very inefficent time complexity which is O(n)^2

Idea

Bubble Sort algorithms sorts a unsorted array as by comparing a swap function to the adjacent element in the array.

1. Smaller number should go on the left side
    if(arr[i]> arr[i+1]){
        swap(arr[i],arr[i+1])
    }

2. If 1st condition is false, you can increase a value of i and j by one to do next comparsion

Bubble Sort vivid example

given array = [5,4,6,8,1]

compare 5 and 4, arr[1] > arr[2] -> swap them [4,5,6,8,1]

compare 5 and 6 -> move on

compare 6 and 8 -> move on

compare 6 and 8 -> move on arr[1] > arr[2] 






In code it looks like this

{% highlight ruby %}

void bubblesort(){

	// easy sorting algorithm to implement
	int temp;
	for(int i = 0; i<n; i++){
		for(int j = 0; j < n-1 - i; j++){ # you do minus i becuase i is already sorted
			if(arr[j] > arr[j+1]){
				temp = arr[j];
				arr[j] = arr[j+1];
				arr[j+1] = temp;
			}
			
		}
	}
	 
}

{% endhighlight %}

