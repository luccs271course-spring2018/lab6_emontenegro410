## Answers

### Q: Why does FixedArrayQueue require an explicit constructor?
A: We need a constructor because `FixedArrayQueue` has a fixed size. Unlike the past lab that used linkedStacks with this lab we have a capacity.

### Q: What happens when you offer an item to a full `FixedArrayQueue`?
A: Once it is full we can't add another item because the Queue has reached its capacity, in this lab its 5.

### Q: What happens when you poll an empty `FixedArrayQueue`?
A: When we poll an empty `FixedArrayQueue`, it will throw `java.util.NoSuchElementException`. Because the Queue is at zero.

### Q: What is the time and (extra) space complexity of each of the FixedArrayQueue methods?
A:
- offer = O(1) b/c we are accessing the index in the array, & array access is O(1).
- peek = O(1) same reason as above. We are justl ook at the first item
- poll = O(1) same reason as above. We are just returning and removing the first item of the queue. we have instant access to the front.
- isEmpty = O(1) same reason as above. We are just seeing if the size is zero which means that the queue is empty.
- size = O(1) same reason as above. We are just looking at a variable and returning it.
- asList = O(n) Iterating through each element and adding it to the list.

