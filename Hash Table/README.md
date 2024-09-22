# Data Structure: Hash Table


This hash table implementation uses chaining as its collision resolution method. When two keys hash to the same index, instead of overwriting, each entry is stored in a sorted doubly linked list at that index. Each list keeps its elements sorted to ensure efficient insertion, search, and deletion. The hash table automatically resizes when the load factor exceeds 0.7, ensuring efficient performance even as the number of entries grows. The hash() function is used to generate hash values for keys, and the sorted linked list provides an elegant solution to handle collisions.


### Member functions

---

```python
	def __init__(self, capacity=32):
```
The initializer for the table defaults the initial table capacity to 32.  It creates a list with capacity elements all initialized to None.

---


```python
	def _resize(self): 
```
This function doubles the hash table's capacity when the load factor exceeds 0.7. It rehashes all existing key-value pairs into the new, larger table to ensure that every entry remains accessible after resizing.



---



```python
	def insert(self, key, value):
```
This function adds a new key-value pair into the table. If a record with matching key already exists in the table, the function does not add the new key-value pair and returns False. Otherwise, function adds the new key-value pair into the table and returns True.  When an insertion causes the HashTable's load factor to exceed 0.7, the list used to store the table must be resized.  Resizing must still allow every existing record to be found.



---

```python
	def modify(self, key, value):
```
This function modifies an existing key-value pair into the table. If no record with matching key exists in the table, the function does nothing and returns False. Otherwise, function changes the existing value into the one passed into the function and returns True

---

```python
	def remove(self, key):
```

This function removes the key-value pair with the matching key.  If no record with matching key exists in the table, the function does nothing and returns False.  Otherwise, record with matching key is removed and returns True

---

```python
	def search(self, key):
```

This function returns the value of the record with the matching key.  If no reocrd with matching key exists in the table, function returns None

---

```python
	def capacity(self):
```
This function returns the number of spots in the table.  This consists of spots available in the table.  

---

```python
	def __len__(self):
```

This function returns the number of Records stored in the table.

---