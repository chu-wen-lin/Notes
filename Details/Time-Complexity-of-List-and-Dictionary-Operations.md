Below I only listed my highly-used operations. Find more information at [Wiki.Python](https://wiki.python.org/moin/TimeComplexity).

### List
|Operation|Example|Time Complexity|Further Explanation|
|---|---|---|---|
|Access|`l[i]`|O(1)||
|Set Item(Update)|`l[i] = new_value`|O(1)||
|Search|`x in l`|O(N)||
|Append|`l.append(x)`|O(1)||
|Insert|`l.insert(i, ele)`|O(N)||
|Pop Last|`l.pop()`|O(1)|
|Pop Intermediate|`l.pop(N/2)`, `N` refers to the length of list|O(N)|Shifts all elements after mid by one slot to the left.(clarify: N/2 elements have to be moved, so the operation is O(N/2))|
|Delete|`del l[i]` |O(N)|Not pythonic!|
|Remove|`l.remove(ele)`|O(N)|remove the "first instance" of that value|
|minimum / maximum|`min(l)` / `max(l)`|O(N)|
|Length|`len(l)`|O(1)|Because the list object maintains an integer counter that increases and decreases as we add and remove elements. Looking up the value of this counter takes constant time.|
|Sort|`l.sort()` / `sorted(l)`|O(nlogN)|Python apply Tim Sort in both `sort()` and `sorted()` functions. By the way, `sort()` is in-place, while `sorted()` returns a new list without affecting the original sequence.|
|Reverse|`l.reverse()` / `reversed(l)` / `l[::-1]`|O(N)|`reverse()`, `reversed()` and `[::-1]` are all linear time, but the first is in-place and the last two are out-place.|
|Slice|`l[i_1: i_2]`|O(i_2 - i_1)|cause we start at i_1 and iterate to i_2|


---
### Dictionary
|Operation|Example|Average Case|Worst Case|Further Explanation|
|---|---|---|---|---| 
|Search|`k in d`|O(1)|O(n) if hash collision happened.|Avoid using `in d.keys()`  if we could, since `d.keys()` lists all the keys and compare each element in this list with our key. In short, `k in d.keys()` finishes in O(n) time while `k in d` finishes in O(1).|
|Access|`d.get(k)`|O(1)|O(n) if hash collision happened.|Better than `d[k]`!! Cause `d[k]` raises a KeyError if the key is not in d.|
|Insert|`d[k]=v`|O(1)|O(n) if hash collision happened.||
|Set Item(Update)|`d[k]=new_value`|O(1)|O(n) if hash collision happened.||
|Pop|`d.pop(k)`|O(1)|O(n) if hash collision happened.||
|Length|`len(d)`|O(1)|O(1)||