### ABC136
[問題ページ](https://atcoder.jp/contests/abc136/tasks)

### A-Transfer
```Swift
func transfer(A: Int, B: Int, C: Int) -> Int {
  return max(0, C - (A - B))
}

print(transfer(A: 6, B: 4, C: 3))

```
