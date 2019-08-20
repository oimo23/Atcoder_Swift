### ABC117
[問題ページ](https://atcoder.jp/contests/abc117/tasks)

### A-Entrance Examination
```Swift
func entranceExamination(T: Int, X: Int) -> Double {
  return Double(T) / Double(X)
}

print(entranceExamination(T: 8, X: 3))

```

### B-Polygon
```Swift
func polygon(N: Int, L: [Int]) -> String {
  guard let max: Int = L.max() else { return "error" }
  let others: Int = L.reduce(0){(m,n) -> Int in m + n}

  return max < others ? "Yes" : "No"
}

print(polygon(N: 4, L: [3, 8, 5, 1]))

```
