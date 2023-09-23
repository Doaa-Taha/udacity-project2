- for this task I used a min-heap to build the huffman tree and to build the min-heap I used a sorted array.
- the reason for using a min-heap is that we'll repeat the removal of every 2 consecutive nodes, sum their frequency and build a new internal node with the sum of the frequency and insert it again to the heap.
- then we heapify ( we need to keep the array sorted ).
- the space complexity is O(k) where k is the number of unique characters in the string to be encoded.
- the time complexity for insertion or removal from min-heap is O(log n) because they have the property of being complete binary tree (CBT). 