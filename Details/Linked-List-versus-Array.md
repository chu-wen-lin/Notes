### Linked List
|Operation|Time Complexity|Further Explanation|
|---|---|---| 
|Access|O(N)|Iterate through each element to reach/find a given element.|
|Search|O(N)|Same as above.|
|Insert|O(1)|O(1) for inserting at the beginning or the end of the linked list. O(n) for inserting at some arbitrary point in between, since we need to reach specific node before insertion.|
|Delete|O(1)|O(1) for deleting the first node or last node. O(n) for deleting at some arbitrary point in between, since we need to reach specific node before deletion.|
---
### Array
|Operation|Time Complexity|Further Explanation|
|---|---|---|
|Access/Update|O(1)|Index helps us to access values/update the existing elements in constant time.|
|Search|O(N)|If the array is sorted, the time complexity reduces to O(logN). Hint: Binary Search|
|Insert|O(N)|After insertion or deletion, we need to move all the values after the affected index. While time complexity of append(adding an item to the end of the list) in list is O(1).|
|Delete|O(N)|If we pop the last element, the time complexity is O(1).|