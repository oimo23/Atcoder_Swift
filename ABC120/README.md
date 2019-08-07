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

```
