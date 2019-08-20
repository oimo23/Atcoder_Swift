### ABC115
[問題ページ](https://atcoder.jp/contests/abc115/tasks)

### A-Christmas Eve Eve Eve
```Swift
func christmasEveEveEve(D: Int) -> String {
  var answer: String = ""

  switch D {
    case 25:
      answer = "Christmas"
    case 24:
      answer = "Christmas Eve"
    case 23:
      answer = "Christmas Eve Eve"
    case 22:
      answer = "Christmas Eve Eve Eve"
    default:
      answer = "Not Christmas"
  }

  return answer
}

print(christmasEveEveEve(D: 14))

```

### B-Christmas Eve Eve
```Swift
func christmasEveEve(N: Int, P: [Int]) -> Int {
  let top: Int = P.reduce(0){(m,n) -> Int in max(m, n)}
  let sum: Int = P.reduce(0){(m,n) -> Int in m + n}

  return sum - (top / 2)
}

print(christmasEveEve(N: 3, P: [4980, 7980, 6980]))

```

