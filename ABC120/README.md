### ABC120
[問題ページ](https://atcoder.jp/contests/abc120/tasks)

### A-Favorite Sound
```Swift
func favoriteSound(A: Int, B: Int, C: Int) -> Int {
  var answer: Int = 0

  if A * C < B {
    answer = C  
  } else {
    answer = Int(floor(Double(B / A)))
  }

  return answer
}

print(favoriteSound(A: 2, B: 11, C: 4))

```

### B-K-th Common Divisor
```Swift
func kthCommonDivisor(A: Int, B: Int, K: Int) -> Int {
  var list: [Int] = [0]
  let smaller: Int = min(A, B)

  for i in 1...smaller {
    if A % i == 0, B % i == 0 {
      list.append(i)
    }
  }

  return list[list.count - K]
}

print(kthCommonDivisor(A: 8, B: 12, K: 2))

```
