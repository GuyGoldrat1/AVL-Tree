# AVL Tree List Project

This project implements an AVL Tree data structure to represent a list. The AVL Tree maintains balance to ensure efficient operations, such as insertion, deletion, and retrieval, which all have logarithmic time complexity.

## Features

1. **AVLNode Class**: Represents a node in the AVL Tree.
    - Attributes: `value`, `left`, `right`, `parent`, `height`, `size`.
    - Methods: 
        - `getLeft()`, `getRight()`, `getParent()`, `getValue()`, `getHeight()`, `getSize()`
        - `setLeft(node)`, `setRight(node)`, `setParent(node)`, `setValue(value)`, `setHeight(h)`, `setSize(s)`
        - `isRealNode()`

2. **AVLTreeList Class**: Implements the AVL Tree List.
    - Attributes: `root`, `virtualNode`, `len`, `firstItem`, `lastItem`
    - Methods:
        - Tree Operations: `insert(i, val)`, `delete(i)`, `retrieve(i)`
        - Tree Properties: `getRoot()`, `empty()`, `length()`, `first()`, `last()`
        - Tree Manipulation: `split(i)`, `concat(lst)`
        - Helpers: `Tree_select(node, i)`, `calculateSize(node)`, `leftRotate(node)`, `rightRotate(node)`, `left_rightRotate(node)`, `right_leftRotate(node)`, `updateHeightNode(node)`, `getBalanceFactor(node)`, `balance(node)`, `rotate(node, child)`, `switchNodes(oldNode, newNode)`, `successor(x)`, `min(node)`, `max(node)`, `listToArray()`

## Usage

### Initialization

To create a new AVL Tree List:

```python
avl_list = AVLTreeList()
```

### Insertion

To insert a value at a specific position:

```python
avl_list.insert(0, "value")  # Insert "value" at position 0
```

### Deletion

To delete a value at a specific position:

```python
avl_list.delete(0)  # Delete the value at position 0
```

### Retrieval

To retrieve a value at a specific position:

```python
value = avl_list.retrieve(0)  # Retrieve the value at position 0
```

### First and Last

To get the first and last values:

```python
first_value = avl_list.first()  # Get the first value
last_value = avl_list.last()    # Get the last value
```

### Length

To get the length of the list:

```python
length = avl_list.length()  # Get the length of the list
```

### List to Array

To convert the AVL Tree List to an array:

```python
array = avl_list.listToArray()  # Convert the list to an array
```

### Split

To split the list at a specific index:

```python
left_tree, value, right_tree = avl_list.split(0)  # Split the list at index 0
```

### Concatenate

To concatenate another AVL Tree List:

```python
avl_list.concat(another_avl_list)  # Concatenate another AVL Tree List
```

## Complexity

- Insertion: \(O(\log n)\)
- Deletion: \(O(\log n)\)
- Retrieval: \(O(\log n)\)
- Split: \(O(\log n)\)
- Concatenation: \(O(\log n)\)

This ensures efficient operations for large lists, maintaining balanced performance across different operations.

## Dependencies

- This implementation requires a `printree` function to visualize the tree structure (not included here).

