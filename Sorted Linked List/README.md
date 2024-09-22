# Data Structure: Sorted Linked List

## Node

The Node class is declared within SortedList.  It stores:
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


