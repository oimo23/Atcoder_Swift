### ABC118
[問題ページ](https://atcoder.jp/contests/abc118/tasks)

### A-B +/- A
```Swift
func bPlusOrMinusA(A: Int, B: Int) -> Int {
  return B % A == 0 ? A + B : B - A
}

print(bPlusOrMinusA(A: 4, B: 12))

```

### B-Foods Loved by Everyone
```Swift
func foodsLovedByEveryone(N: Int, M: Int, KA: [[Int]]) -> Int {
  var answer: Int = 0

  for i in 1...M {
    var flg: Int = 0

    for j in 0..<N {
      let liked = KA[j][1..<KA[j].count]

      if(liked.filter{$0==i}.count > 0) {
        flg += 1
      }
    }

    if flg == N {
      answer += 1
    }
  }

  return answer
}

print(foodsLovedByEveryone(N: 3, M: 4, KA: [[2, 1, 3], [3, 1, 2, 3], [2, 3, 2]]))

```
