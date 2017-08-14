
## Solution
https://www.codewars.com/kata/find-the-odd-int/train/python


### My Solution
```javascript
//javascript
function findOdd(A) {
	var n = 0;
	A.forEach( v => n = n^v )
	return n
}
```

```python
//python
from functools import reduce
def find_it(seq):
    return reduce((lambda x, y: x^y), seq)
```


### Best Solution
```javascript
//javascript
const findOdd = (xs) => xs.reduce((a, b) => a ^ b);
```

```python
//python
import operator
def find_it(xs):
    return reduce(operator.xor, xs)
```
