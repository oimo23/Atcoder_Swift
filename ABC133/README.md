### ABC133
[問題ページ](https://atcoder.jp/contests/abc133/tasks)

### A-T or T
```Swift
func torT(N: Int, A: Int, B: Int) -> Int {
  let train = N * A
  let bus   = B

  return min(train, bus)   
}

```

### B-Good Distance
```Swift
func goodDistance(N: Int, D: Int, X: [[Int]]) -> Int {
  let points: [Array] = X
  var cnt: Int = 0;

  for i in 0..<N {
    for j in i+1..<N {
      var distance:Int = 0

      for k in 0..<points.count-1 {
        distance += (points[i][k] - points[j][k]) * (points[i][k] - points[j][k])
      }

      let sqrted:Double = sqrt(Double(distance));

      // 小数点切り捨てたものが元の数字と一緒なら整数である
      if sqrted == floor(sqrted) {
        cnt += 1
      }
    }
  }

  return cnt
}

print(goodDistance(N: 3, D: 2, X: [[1,2], [5,5], [-2,8]]))

```
