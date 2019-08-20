### ABC121
[問題ページ](https://atcoder.jp/contests/abc121/tasks)

### A-White Cells
```Swift
func whiteCells(H: Int, W: Int, h: Int, w: Int) -> Int {
  return (H * W) - (h * W) - ((w * H) - (h * w))
}

print(whiteCells(H: 3, W: 2, h: 2, w: 1))

```

### B-Can you solve this?
```Swift
func canYouSolveThis(N: Int, M: Int, C:Int, B: [Int], A: [[Int]]) -> Int {
  var cnt: Int = 0

  for i in 0..<N {
    var temp: Int = 0

    for j in 0..<A[i].count {
      temp += A[i][j] * B[j]
    }

    if temp + C > 0 {
      cnt += 1
    }
  }

  return cnt
}

print(canYouSolveThis(N: 2, M: 3, C:-10, B: [1, 2, 3], A: [[3, 2, 1], [1, 2, 2]]))

```
