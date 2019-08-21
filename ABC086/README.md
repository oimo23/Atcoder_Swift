### ABC086
[問題ページ](https://atcoder.jp/contests/abc086/tasks)

### A-Product
```Swift
func product(A: Int, B: Int) -> String {
  return ((A * B) % 2 == 0 ? "Even" : "Odd");
}

print(product(A: 2, B: 3))

```

### B-1 21
```Swift
func oneTwoOne(A: String, B: String) -> String {
  let N: Int = Int(A + B) ?? 0
  var answer: String = "No"

  for i in 1..<N {
    if i * i == N {
      answer = "Yes"
      break
    }
  }

  return answer
}

print(oneTwoOne(A: "1", B: "21"))

```