## KeyPoints

Notes to store and future references.

* Arraylist increses the array dynamically, as

  ​		 1+2+4+8+.....+x = x+x/2+x/4+......+4+2+1 = O(2x)

  >  <b>x insertion takes O(2x) time. The amortized time for each insertion is O(1).</b>

* Binary Search

  > In sorted N element array, searching for an element out finding the mid and validating left or right  and repeating the process on remainig element 
  >
  > N=16 
  >
  > N=8.  /* divided by 2 */
  >
  > N=4. /* divided by 2 */
  >
  > N=2  /* divided by 2 */
  >
  > N=1  /* divided by 2 */
  >
  > So 16 to reach 1 is done in K steps i.e $2^k$ = N, k = log N

  * when ever you see no of elements gets halved each time, that will likely be O(log N)

* F(n) = (n< 1) ? 1 : f(n-1)+f(n-1)

     NOTE: When you have recursive function that makes multiple calls, the runtime will often(but not always) look like O($branches^depth$  ), where branches is the number if times each recursive call branches. in this case, this gives us )($2^N$)