Task: Consider how the remove operation for doubly-linked lists is different from singly-linked lists. Write 3-5 sentences in your README explaining the significant differences.
The time complexity is almost the same as both functions would still have one loop. However, in doubly-linked lists, you have to change both the "next" and "prev" values while in singly-linked lists there is only the "next" pointer. Also, for singly-linked list remove operations, you have to keep track of the previous item in the list because you don't have the prev functionality. This means it requires 1-2 extra computations per loop iteration, but the time complexity is O(n). 






Task: Before beginning to code, compare and contrast the optimal runtimes of each method with one another. Which methods do we expect to take longer with larger inputs? Which methods do we expect to take the same amount of time no matter the input? Write your thoughts in your README.
The general notion is that the functions that contain loops will take longer as the input gets larger because for methods like get(), reverse(), remove(), getNode(), and removeNode(), they will have to traverse the entire linked list to complete their operations. As for functions like removeFirst(), removeLast(), getFirst(), getLast(), addFirst(), addLast(),  their operations require them to do their respective operations on the head or tail of a linked list which only requires 1 operation, hence an O(1) time complexity.  




Task: Consider the new removeNode method. Does it have the same runtime as the remove method? Explain why or why not in your README.
The removeNode() method has the same runtime (a worst case of O(n) where n is the input size) because they contain the same exact loop with the same while conditioning. Furthermore, the functions perform the same task with different outputs, therefore they have the same runtime.