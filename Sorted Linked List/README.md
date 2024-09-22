# Data Structure: Sorted Linked List

## Class: Node

The Node class is declared within SortedList. It stores:
* a piece of data
* a reference to the next Node in the SortedList (None if Node is last node)
* a reference to the previous Node in the SortedList (None if Node is first node)
    
When a Node is initialized, it is passed a data value.  Optionally it is also passed a reference to the next node and a reference to the previous node (in that order).  If the data values are not passed in, they are defaulted to None.

The Node function has the following member functions:

---

```python
def get_data(self)
```
function returns data stored in node

---

```python
def get_next(self)
```
function returns reference to next node in SortedList

---

```python
def get_previous(self)
```
function returns reference to previous node in SortedList

---

## Class: SortedList

A SortedList is a sorted doubly linked list. 


A sorted linked list is a linked list where values stay sorted from smallest to biggest with the smallest node at the front of the list and the largest node at the back.

When the SortedList is first created it is empty.

The SortedList has the following member functions

```python
def get_front(self)
```
This function returns a reference to the first data node in the list.  If list is empty, function returns None

---

```python
def get_back(self)
```
This function returns a reference to the last data node in the list.  If list is empty, function returns None

---

```python  

def is_empty(self)
```
This function returns True if the list is empty, False otherwise

---


```python
def __len__(self)
```
This function returns the number of values stored in the list

---

```python
def insert(self,data)
```
this function inserts data into the list such that the list stays sorted. You may assume that the data being added can be compared using comparison operators.  Function returns reference to newly added node.

---

```python
def erase(self, node)
```
This function removes the node referred to by the node argument.   This function returns nothing. If node is None, function does not alter list and will raise the ValueError with this statement:

```python
  raise ValueError('Cannot erase node referred to by None')
```

---

```python
def search(self, data)
```
This function returns a reference to the node containing data if it exists within the list, None if no node contains data



