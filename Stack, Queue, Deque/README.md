# Data Structures: Stack, Queue, Deque

### Class: Stack

The Stack class implements a FILO data structure.  This class must be implemented using a python list (not a linked list) based solution.


```python
def __init__(self, cap):
```
This function initializes the Stack class data members. It is passed a value representing it's capacity, with a default capacity of 10 if no capacity is passed in.

---


```python
def capacity(self):
```
This function returns capacity.  

Runtime requirement for this function is O(1)

---


``` python
def push(self, data):
```
This function adds data to the "top" of the Stack.  function does not return anything.  When this operation causes the number of items stored to exceed the current capacity, a resizing operation will need to take place.  Resizing always doubles the current capacity of the array.


Runtime requirement for this function is O(1) when no resizing occurs, O(n) when resizing occurs


---

``` python
def pop(self):
```
This function removes the newest value from the Stack (the value at the "top" of the Stack).  function returns value removed.  

If the function is called on an empty Stack, raise the IndexError with this statement

```python
raise IndexError('pop() used on empty stack')
```


Runtime requirement for this function is O(1)

---

``` python
def get_top(self):
```
This function returns the the newest value (value at "top") from the Stack without removing it.  Function returns None if stack is empty 

Runtime requirement for this function is O(1)

---

``` python

  def is_empty(self):
```
This function returns True if Stack is empty, False otherwise.  

Runtime requirement for this function is O(1)


---

``` python

  def __len__(self):
```
This function returns the number of values in the Stack.  

Runtime requirement for this function is O(1)

### Class: Queue

The Queue class implements a FIFO data structure.  This class must be implemented using a python list (not a linked list) based solution.


```python
def __init__(self, cap):
```
This function initializes the Queue class data members. It is passed a value representing it's capacity, with a default capacity of 10 if no capacity is passed in.

---

```python
def capacity(self):
```
This function returns capacity.

Runtime requirement for this function is O(1)

---

``` python
def enqueue(self, data):
```
This function adds data to the "back" of the Queue.  function does not return anything.  When this operation causes the number of items stored to exceed the current capacity, a resizing operation will need to take place.  Resizing always doubles the current capacity of the array.


Runtime requirement for this function is O(1) when no resizing occurs, O(n) when resizing occurs

---

``` python
def dequeue(self):
```
This function removes the oldest value from the Queue (the value at the "front" of the Queue).  Function returns value removed.  

If the function is called on an empty Queue, raise the IndexError with this statement

---

```python
raise IndexError('dequeue() used on empty queue')
```


Runtime requirement for this function is O(1)

---

``` python
def get_front(self):
```
This function returns the the oldest value (value at "front") from the Queue without removing it. Function returns None if Queue is empty.

Runtime requirement for this function is O(1)

---

``` python

def is_empty(self):
```
This function returns True if Queue is empty, False otherwise.  Runtime requirement for this function is O(1)

---

``` python

def __len__(self):
```
This function returns the number of values in the Queue.  Runtime requirement for this function is O(1)



### Class: Deque


A Deque is a double ended queue.  This class allows you to add/remove items from front or the back of the data structure.  This class must be implemented using a python list (not a linked list) based solution.  

```python

def __init__(self, cap):
```
This function initializes the Deque class data members. It is passed a value representing it's capacity, with a default capacity of 10 if no capacity is passed in.


```python
def capacity(self):
```
This function returns capacity

Runtime requirement for this function is O(1)

---

``` python
def push_front(self, data):
```
This function adds data to the "front" of the Deque.  Function does not return anything.  When this operation causes the number of items stored to exceed the current capcity, a resizing operation will need to take place.  Resizing always doubles the current capcity of the array.


Runtime requirement for this function is O(1) when no resizing occurs, O(n) when resizing occurs

---

``` python
def pop_front(self):
```
This function removes the  value from the "front" of the Deque. Function returns value removed.  


If the function is called on an empty Deque, raise the IndexError with this statement


```python
raise IndexError('pop_front() used on empty deque')
```

Runtime requirement for this function is O(1)

---

``` python
def push_back(self):
```
This function adds data to the "back" of the Deque.  Function does not return anything.  When this operation causes the number of items stored to exceed the current capcity, a resizing operation will need to take place.  Resizing always doubles the current capcity of the array.


Runtime requirement for this function is O(1) when no resizing occurs, O(n) when resizing occurs

---
``` python
def pop_back(self):
```
This function removes the  value from the "back" of the Deque. Function returns value removed.  

If the function is called on an empty Deque, raise the IndexError with this statement


```python
  raise IndexError('pop_back() used on empty deque')
```


Runtime requirement for this function is O(1)

---

``` python
  def get_front(self):
```
This function returns the value from the "front" of the Deque without removing it.  Runtime requirement for this function is O(1)

---

``` python
  def get_back(self):
```
This function returns the value from the "back" of the Deque without removing it.  Runtime requirement for this function is O(1)

---

``` python

def is_empty(self):
```
This function returns True if Deque is empty, False otherwise.  Runtime requirement for this function is O(1)

---

``` python
def __len__(self):
```
This function returns the number of values in the Deque.  Runtime requirement for this function is O(1)

---


``` python
def __getitem__(self, k):
```
This function returns the k'th value from the "front" of the Deque without removing it.  For example, if k == 0, this function would return the item at front of the Deque.  if k == 1, function would return the second item from the of the front item of the Deque.  


If k is out of range, raise the IndexError exception using the statement:

```python
raise IndexError('Index out of range')
```

Runtime requirement for this function is O(1)

---
