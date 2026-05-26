Time complexity of an algorithm - estimates how much time the algorithm will use for some input. 
denoted by O(...), the three dots represent some function
n -- denotes the input size

Loops - common reason for the algorithm to be slow is that it contains many loops the go through the input. 
the more nested loops the algorithm contains, the slower it is. 
if there are k nested loops, the time complexity is $O(n^k)$ 

Phases - if the algorithm consists of consecutive phases, the total time complexity is the largest time complexity of a single phase. 
for example, if a certain code has time complexities $O(n)$, $O(n^2)$, and $O(n)$, the total time complexity is $O(n^2)$ -- others are usually considered the bottlenecks of the code

Several variables - when time complexity contains several variables
for example, the time complexity for the following code is $O(nm)$ 
```
for (int i = 1; i <= n; i++) {
	for(int j = 1; j <= m; j++) {
		//code
	}
}
```

Recursion - 

$O(1)$ the running time of a constant-time algorithm does not depend on the input size. A typical constant-time algorithm is a direct formula that calculates the answer. 

$O(\log n)$ a logarithmic algorithm often halves the input size at each step. the running time of such an algorithm is logarithmic, because $\log_2 n$ equals the number of times n must be divided by 2 to get 1

$O(\sqrt n)$ a square root algorithm is slower than $O(\log n)$ but faster than $O(n)$. a special property of square roots is that $\sqrt n = n / \sqrt n$, so the square root $\sqrt n$ lies, in some sense, in the middle of the input

