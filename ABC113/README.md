### ABC113
[問題ページ](https://atcoder.jp/contests/abc113/tasks)

### A-Discount Fare
```Swift
func discountFare(X: Int, Y: Int) -> Int {
  return X + (Y / 2)
}

print(discountFare(X: 81, Y: 58))

```

### B-Palace
```Swift
func palace(N: Int, T: Double, A: Double, H: [Double]) -> Int {
  var diffs: [Double] = []

  for i in 0..<H.count {
    let Haverage: Double = T - (H[i] * 0.006)
    diffs.append(abs(A - Haverage))
  }

  let minDiff: Double = diffs.min() ?? 0
  let answer:  Int = diffs.firstIndex(of: minDiff) ?? 0

  return answer + 1
}

print(palace(N: 2, T: 12, A: 5, H: [1000, 2000]))

```
