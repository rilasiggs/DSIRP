# Exercise
1.  What is the order of growth of $n^3 + n^2$? What about $1000000 n^3 + n^2$? What about $n^3 + 1000000 n^2$?

        The order is Cubic because the leading term, $n^3$ is cubic.

2.  What is the order of growth of $(n^2 + n) \cdot (n + 1)$? Before you start multiplying, remember that you only need the leading term.

        The order is cubic. When multiplied out, the leading term will be $n^3$.

3.  If $f$ is in $O(g)$, for some unspecified function $g$, what can we say about $af+b$, where $a$ and $b$ are constants?

        $af+b$ will still be in $O(g)$. Scaling the function and adding a constant will not change the leading term.

4.  If $f_1$ and $f_2$ are in $O(g)$, what can we say about $f_1 + f_2$?

        $f_1 + f_2$ will still be in $O(g)$.

5.  If $f_1$ is in $O(g)$ and $f_2$ is in $O(h)$, what can we say about $f_1 + f_2$?

        $f_1 + f_2$ will be in whichever fuction has a higher order of growth.

6.  If $f_1$ is in $O(g)$ and $f_2$ is in $O(h)$, what can we say about $f_1 \cdot f_2$?

        It will belong to $O(gh)$.

# Sorting
1.  What is a "comparison sort?" What is the best worst-case order of growth for a comparison sort? What is the best worst-case order of growth for any sort algorithm?

        A comparison sort reads each element through one comparison operation. The best case is $n$ and the worst case is $n^2$.

2.  What is the order of growth of bubble sort, and why does Barack Obama think it is "the wrong way to go?"

        $n^2$. Bubble sorts are only used on small data sets because the ineffecieny becomes too large when computing lots of data.

3.  What is the order of growth of radix sort? What preconditions do we need to use it?

        $O(nk)$ where n is the amount of numbers and k is the number of digits. We need to know both n and k before using it.

4.  What is a stable sort and why might it matter in practice?

        A stable sort does not change the order of input and output in specific cicrumstances. This is usefull when you want to perform multiple sorts.

5.  What is the worst sorting algorithm (that has a name)?

        Bogosort is the worst sorting algorithm. It could sort forever.

6.  What sort algorithm does the C library use? What sort algorithm does Python use? Are these algorithms stable? You might have to Google around to find these answers.

        C uses bubble sort, selection sort, quick sort, merge sort, heap sort and insertion sort. Python uses Tim sort, a combination of insertion sort and merge sort. Tim sort is stable and so are the C algorithms.

7.  Many of the non-comparison sorts are linear, so why does Python use an $O(n \log n)$ comparison sort?

        It is able to handle much more complex data sets.