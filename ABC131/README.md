### ABC131
[問題ページ](https://atcoder.jp/contests/abc131/tasks)

### A-Security
```Swift
func security(S: String) -> String {
  let s: [String] = stringToArray(str: S)

  for i in 0..<s.count-1 {
    if s[i] == s[i+1] {
      return "Bad"
    }
  }

  return "Good"
}

print(security(S: "8080"))

```

### B-Bite Eating
```Swift

```