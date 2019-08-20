### ABC125
[問題ページ](https://atcoder.jp/contests/abc125/tasks)

### A-Biscuit Generator
```Swift
func biscuitGenerator(A: Int, B: Int, T: Int) -> Int {
  return Int(floor(Double(T / A))) * B
}

print(biscuitGenerator(A: 3, B: 2, T: 9))

```

### B-Resale
```Swift
func resale(N: Int, V: [Int], C: [Int]) -> Int {
  var answer: Int = 0

  for i in 0..<N {
    if V[i] - C[i] >= 0 {
      answer += V[i] - C[i]
    }
  }

  return answer
}

print(resale(N: 3, V: [10, 2, 5], C: [6, 3, 4]))

```
