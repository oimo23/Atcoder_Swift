### ABC135
[問題ページ](https://atcoder.jp/contests/abc135/tasks)

### A-Harmony
```Swift
func harmony(A: Int, B: Int) -> String {
  if(A % 2 != B % 2) {
    return "IMPOSSIBLE"
  }

  let answer: Int = (A + B) / 2

  return String(answer)
}

print(harmony(A: 2, B: 16))

```

### B-0 or 1 Swap
```Swift
func zeroOrOneSwap(N: Int, P: [Int]) -> String {
  var modelArray: [Int] = [Int](repeating: 0, count: N)
  var answer: String
  var diff: Int = 0

  for i in 0..<N {
    modelArray[i] = i + 1
  }

  for i in 0..<N {
    if modelArray[i] != P[i] {
      diff += 1
    }
  }

  if diff == 0 || diff == 2 {
    answer = "YES"
  } else {
    answer = "NO"
  }

  return answer
}

print(zeroOrOneSwap(N: 5, P:[5, 2, 3, 4, 1]))

```
