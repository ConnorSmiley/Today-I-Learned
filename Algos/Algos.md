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

























