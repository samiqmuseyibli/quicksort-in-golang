# Quick sort in Golang (Go Programming Language)


<h3>Time Complexity</h3>
    * Best complexity: `n*log(n)`
    * Average complexity: `n*log(n)`
    * Worst complexity: `n^2`

<h4>Quick sort implementation steps:</h4>
<h5>Let's take the input array as <b>{15, 3, 12, 6, -9, 9, 0}</b> and we can see how the Quick sort is sorting the array.</h5>

* Choose the lowest or highest index value as a pivot element, in our above example we chose the lowest index as a pivot element 15.
* Declare two variables (i.e. pointer) to store the lowest and highest index position except the pivot element, so the lowest index position is 1 points the value 3 and the highest index position is 6 which is pointing the value 0
* Move the left side pointer towards right until the value of the pointer is less than or equal to the pivot element.
* Move the right side pointer towards left until the value of the pointer is greater than the pivot element.
* Interchange the values of left side pointer and right side pointer.
* Interchange the values of leftmost index (i.e. position 0 has the pivot element 15) and right side pointer.
* The right side pointer is a new pivot position for the value 15
* Split the array into two sub-arrays with the help of pivot point
  * Index from 0 to pivot
  * Index from (pivot + 1) to (n - 1), where n is the length of an array
* Apply the step 1 to 8 until there is no more elements to split as an array.