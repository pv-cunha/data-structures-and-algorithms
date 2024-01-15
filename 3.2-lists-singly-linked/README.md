# Singly Linked List in Java

A Singly Linked List is a basic data structure in Java, consisting of a series of nodes linked together in a sequence. Each node in a linked list contains data and a reference to the next node.

## Understanding Singly Linked Lists

### Components

- **Node**: The fundamental part of a linked list. Each node contains:
    - **Data**: The value or data stored in the node.
    - **Next**: A reference to the next node in the list.

- **Head**: The first node in the list, used as the starting point for any traversal or operation.

- **Tail**: The last node in the list, which points to `null`, indicating the end of the list.

- **Traversal**: To access elements, start from the head and follow the `next` references.

## Operations

- **Insertion**: Add a new node at the beginning, end, or after a specific node.
- **Deletion**: Remove a node by adjusting the `next` pointers of adjacent nodes.
- **Search**: Find a node with a particular value.
- **Traversal**: Visit each node to perform operations like displaying node values.

## Advantages and Disadvantages

- **Advantages**:
    - **Dynamic Size**: Can grow or shrink as needed.
    - **Efficient Insertions/Deletions**: More efficient than arrays in certain scenarios.

- **Disadvantages**:
    - **Sequential Access**: No direct access to elements by their position.
    - **Extra Memory**: Each node requires additional memory for the `next` pointer.

## Implementation in Java

```java
class Node {
    int data;
    Node next;

    public Node(int data) {
        this.data = data;
        this.next = null;
    }
}

class SinglyLinkedList {
    Node head;

    public void add(int data) {
        Node newNode = new Node(data);
        if (head == null) {
            head = newNode;
        } else {
            Node current = head;
            while (current.next != null) {
                current = current.next;
            }
            current.next = newNode;
        }
    }
}
