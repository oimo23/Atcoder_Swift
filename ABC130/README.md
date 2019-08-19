### ABC130
[問題ページ](https://atcoder.jp/contests/abc130/tasks)

### A-Rounding
```Swift
func rounding(X: Int, A: Int) -> Int {
  return X < A ? 0 : 10
}

print(rounding(X: 7, A: 5))

```

### B-Bounding
```Swift
func bounding(N: Int, X: Int, Ls: [Int]) -> Int {
  var list: [Int] = []

  for i in 0...N {
    if i == 0 {
      list.append(0)
    } else {
      let temp = list[i-1] + Ls[i-1]
      list.append(temp)
    }
  }

  return list.filter{$0 <= X}.count
}

print(bounding(N: 3, X: 6, Ls: [3, 4, 5]))

```
