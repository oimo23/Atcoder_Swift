### ABC127
[問題ページ](https://atcoder.jp/contests/abc127/tasks)

### A-Ferris Wheel
```Swift
func ferrisWheel(A: Int, B: Int) -> Int {
  var answer:Int = 0

  if A > 12 {
    answer = B
  } else if A > 5 {
    answer = B / 2
  }

  return answer
}

print(ferrisWheel(A: 12, B: 100))

```

### B-Algae
```Swift

```
