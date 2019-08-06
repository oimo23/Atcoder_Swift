### ABC132
[問題ページ](https://atcoder.jp/contests/abc132/tasks)

### A-Fifty-Fifty
```Swift
func fiftyFifty(S: String) -> String {
  for s in S {
    let duplicateCnt:Int = S.filter{$0==s}.count
    
    if duplicateCnt != 2 {
      return "No"
    }
  }

  return "Yes"
}

print(fiftyFifty(S: "ASSA"))

```

### B-Ordinary Number
```Swift
func ordinaryNumber(N: Int, P: [Int]) -> Int {
  var cnt: Int = 0

  for i in 1..<N-1 {
    let left   = P[i-1]
    let center = P[i]
    let right  = P[i+1]

    let maxValue = max(left, center, right)
    let minValue = min(left, center, right)

    if(maxValue != center && minValue != center) {
      cnt += 1
    }
  }

  return cnt
}

print(ordinaryNumber(N: 5, P: [1, 3, 5, 4, 2]))

```
