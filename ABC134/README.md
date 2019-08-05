### ABC134
[問題ページ](https://atcoder.jp/contests/abc134/tasks)

### A-Dodecagon
```Swift
func dodecagon(r: Int) -> Int {
  let answer: Int = 3 * (r * r)
  
  return answer
}

print(dodecagon(r: 4))

```

### B-Golden Apple
```Swift
func goldenApple(N: Double, D: Double) -> Int {
  let viewRange: Double = (D * 2) + 1
  let answer: Double = ceil(N / viewRange)

  return Int(answer)
}

print(goldenApple(N: 6, D: 2))

```
