### ABC129
[問題ページ](https://atcoder.jp/contests/abc129/tasks)

### A-Airplane
```Swift
func airplane(P: Int, Q: Int, R: Int) -> Int {
  let times: [Int] = [P, Q, R].sorted{$0 < $1}

  return times[0] + times[1]
}

print(airplane(P:1, Q:3, R:4))

```

### B-Balance
```Swift

```
