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
func balance(N: Int, W: [Int]) -> Int {
  var right: Int = W.reduce(0){(m,n) -> Int in m + n}
  var left: Int  = 0
  var answer: Int = right

  for i in 0..<W.count {
    left  += W[i]
    right -= W[i]

    answer = min(answer, abs(left - right))
  }

  return answer
}

print(balance(N: 4, W: [1, 3, 1, 1]))

```
