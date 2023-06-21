> ## 

```javascript

``` 







> ## Bubble Sort
#### Swaps many to move largest to end
#### Great for nearly-sorted data

```javascript


``` 





> ## Selection Sort
#### One swap at the end of each loop
#### Minimal Swaps, but bad performance

```javascript
const selection = (input) => {
    for (let i = 0; i < input.length; i++){
        let low = i
        for (let d = i + 1; d < input.length; d++){
            if (input[low] > input[d]) {
                low = d
            }
        }
        if (i !== low) {
            let temp = input[i]
            input[i] = input[low]
            input[low] = temp
        }
    }
    return input
}

```



> ## Insertion Sort
#### 
#### Best for continuous data, nearly sorted data
###### Time = Best : O(n) | Avg : O(n)**2 | Worst : O(n)**2
##### Space O(1)


```javascript
const insertionSort = (input) => {
    for (let i = 0; i < input.length; i++){
        let currentVal = input[i]
        for (let d = i-1; d >= 0 && input[d] > currentVal; d--){
            input[d+1] = input[d]
        }
        input[d+1] = currentVal
    }
    return input
}
``` 





> ## Merge Sort
#### 
#### 
###### 


```javascript
const merge = (input1, input2) => {
    let results = []
    let i = 0
    let d = 0
    while (i < input1.length && d < input2.length){
        if(input1[i] > input2[d]) {
            results.push(input1[i])
            i++
        } else {
            results.push(input2[d])
            d++
        }

        while (i < input1.length) {
            results.push(input1[i])
            i++
        }
        while (d < input2.length) {
            results.push(input2[d])
            d++
        }
    }
    return results
}
``` 







> ## Merge Sort Recursion
#### 
#### Time =  Best : O(n log n) | Avg : O(n log n) | Worst : O(n log n)
###### Space Compx = O(n)


```javascript
const merge = (input) => {
    if(input.length <= 1) return input
    let mid = Math.floor(input.length/2)
    let left = merge(input.slice(0,mid))
    let right = merge(input.slice(mid))
    return merge(left, right)
}
``` 






> ## Quick Sort
#### 
#### Time = Best, Avg: O(n log n) | Worst O(n**2)
###### Space Compx = O(log n)


```javascript
const x = (arr, start = 0, end = arr.length + 1) => {
    const swap = (array, i, d) => {
        let temp = array[i]
        array[i] = array[d]
        array[d] = temp
    }

    let pivot = arr[start]
    let swapIdx = start

    for (let i = start+1; i < arr.length; i++){
        if(pivot > arr[i]) {
            swapIdx++
            swap(arr, swapIdx, i)
        }
    }
    swap(arr, start, swapIdx)
    return swapIdx
}

const quicksort = (arr, left = 0, right = arr.length - 1) => {
    if (left < right) {
        let pivotIndex = x(arr, left, right)

        quicksort(arr,left, pivotIndex-1)
        quicksort(arr,pivotIndex+1,right)
    }
    return arr
}
``` 





> ## Radix Sort
#### 
#### Time = O(nk)
###### Space Compx = O(n + k)


```javascript
const getDigit = (num, i) => {
    return Math.floor(Math.abs(num) / Math.pow(10, i)) % 10
}

const digitCount = (num) => {
    if (num === 0) return 1
    return Math.floor(Math.log10(Math.abs(num))) + 1
}

const mostDigits = (nums) => {
    let maxDigits = 0
    for (let i = 0; i < nums.length; i++){
        maxDigits = Math.max(maxDigits, digitCount(nums[i]))
    }
    return maxDigits
}

const radixSort = (nums) => {
    let maxDigitCount = mostDigits(nums)
    for (let d = 0; d < maxDigitCount; d++){
        let digitBuckets = Array.from({length:10}, () => [])
        for (let i = 0; i < nums.length; i++){
            let digit = getDigit(nums[i], k)
            digitBuckets[digit].push(nums[i])
        }
        nums = [].concat(...digitBuckets)
    }
}

``` 








> ## Graphs
#### 
#### Time = 
###### Space Compx = 


```javascript
class Graph {
constructor() {
this.adjacenyList = {}
}
addVertex(vertex) {
if(!this.adjacenyList[vertex]) this.adjacenyList[vertex] = []
}
addEdge(v1, v2) {
this.adjacenyList[v1].push(v2)
this.adjacenyList[v2].push(v1)
}
removeEdge(v1, v2) {
// if(v1) {
//    this.adjacenyList[v1].pop(v1)
// }
// if (v2) {
//     this.adjacenyList[v2].pop(v2)
// }
this.adjacenyList[v1] = this.adjacenyList[v1].filter(x => x !== v2)
this.adjacenyList[v2] = this.adjacenyList[v2].filter(x => x !== v1)
}
removeVertex(vertex){
for (let i = 0; i < this.adjacenyList[vertex].length; i++){
const adj = this.adjacenyList[vertex].pop()
this.removeEdge(vertex, adj)
}
delete this.adjacenyList[vertex]
}
}

const graph = new Graph()
graph.addVertex("Tokyo")
graph.addVertex("Texas")
graph.addVertex("NewYork")
graph.addVertex("Cali")

graph.addEdge("Texas", "Tokyo")
graph.addEdge("Texas", "Cali")
// graph.removeEdge("Texas", "Tokyo")
// graph.removeEdge("Tokyo", "Texas")
// graph.removeEdge("Cali", "Texas")

graph.removeVertex("Tokyo")

console.log(graph)

``` 







> ## Stack Link-list

### First IN / Last Out

#### Insertion - O(1)
#### Removal - O(1)
#### Searching - O(n)
#### Access - O(n)

#### Time =
###### Space Compx =

```javascript
class Node {
    constructor(value) {
        this.value = value
        this.next = null

    }
}

class Stack {
    constructor() {
        this.first = null
        this.last = null
        this.size = 0

    }
    push(val) {
        const newNode = new Node(val)
        if (!this.first) {
            this.first = newNode
            this.last = newNode
        } else {
            let temp = this.first
            this.first = newNode
            this.first.next = temp
        }
        return ++this.size
    }
    pop() {
        if(!this.first) return null
        let temp = this.first
        if(this.first === this.last) {
            this.last = null
        }
        this.first = this.first.next
        this.size--
        return temp.value
    }
}


const stack = new Stack()

stack.push("a")
stack.push("b")
stack.push("c")
stack.push("d")
console.log(stack)
stack.pop()
console.log(stack)
stack.pop()
console.log(stack)
stack.pop()
console.log(stack)
stack.pop()
console.log(stack)
``` 









> ## Queue Linked-list

### First IN / First Out

#### Insertion - 
#### Removal - 
#### Searching - 
#### Access - 

#### Time =
###### Space Compx =

```javascript
class Node {
    constructor(value) {
        this.value = value
        this.next = null
    }
}

class Queue {
    constructor() {
        this.first = null
        this.last = null
        this.size = 0
    }

    enqueue(val) {
        let newNode = new Node(val)
        if (!this.first) {
            this.first =  newNode
            this.last = newNode
        } else {
            this.last.next = newNode
            this.last = newNode
        }
        return ++this.size
    }

    dequeue() {
        if(!this.first) return null
        let temp = this.first
        if(this.first === this.last) {
         this.last = null
        }
        this.first = this.first.next
        this.size--
        return temp.value
    }
}


const q = new Queue()
q.enqueue('a')
q.enqueue('b')
q.enqueue('c')
q.enqueue('d')
q.dequeue()

console.log(q)

``` 








































































