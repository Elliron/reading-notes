# Stacks and Queues

- Stack - data structure consisting of Nodes
- Nodes - references the next Node in the stack but not the previous node
    - Push - Nodes or items are put into stack.
        - O(1) - Takes same amount of time regardless of Nodes (n) in stack.
        - Make Node with value and next
        - assign next of new node to the previous top node in stack
        - reassign top reference to new node
    - Pop - removed from the stack (empty exception raised)
        - O(1) 
        - Top node is removed and the next node in stack is reassigned to be the new top.
        - Check IsEmpty first
        - Create temp reference that points to same Node as top
        - Re-assign top to next node in list
        - Clear temp reference
        - Remove top node
        - return value temp node popped off
    - Top - top of stack
    - Peek - view value on top of the stack (empty stack exception raised)
        - O(1)
        - check IsEmpty first
    - IsEmpty - returns true when stack is empty otherwise false
        - O(1)
- FILO - First In Last Out - first item added is the last item popped out
- LIFO - Last In First Out - last item added is the first item popped out

    - Enqueue - Add item to queue
        - O(1)
        - Change next property of the last node to the value of the node being added
        - Reassign rear reference to the new node

    - Dequeue - remove item from queue
    - O(1)
    - Removes front node
    - Check IsEmpty First
    - Create a Temporary reference named temp and point it towards the fist node.
    - Reassign front to the second node in the stack.
    - Reassign next propery on temp node to null.
    - Return vlue of temp Node

    [Home](../README.md)
