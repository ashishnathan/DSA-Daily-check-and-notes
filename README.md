# DSA-Daily-check-and-notes

Day 1

Data Structures - organization of data to access it efficiently.

Algorithm - a step-by-step set of operations to solve a specific problem or a set of problems

Types of data structures - 
- Linear (stack, array, linked list)
- non-linear (tree, graph)
- Static (compile time memory allocation) for faster access, but slow insertion and deletion
- dynamic (runtime memory allocation) for faster insertion/deletion but slow access to elements

Recursion -
- case wherein the function calls for itself
- there must be a defined case for stopping the loop or else would lead to stack overflow
- when the loop is closed and the function calls itself until defined limits, it becomes a recursion tree
- Code Snippet for simple recursion example of calling your name n times over (n user-defined)
```
#include <iostream>
using namespace std;

int cnt = 0;
void print(int n) {
    if (cnt == n) return;
    cout << "Ashish" << endl;
    cnt++;
    print(n);
}
int main() {
    int n;
    cin >> n;
    print(n);
    return 0;
}
```
- Code snippet for sum of all n numbers using recursion
```
#include <iostream>
using namespace std;

void add(int i, int sum) {
    if (i < 1) {
        printf("%d", sum);
        return;
    }
    add(i-1, sum+i);
}

int main() {
    int i;
    cin >> i;
    add(i, 0);
}
```
- 
