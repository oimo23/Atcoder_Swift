### ABC126
[問題ページ](https://atcoder.jp/contests/abc126/tasks)

### A-Changing a Character
```Swift
func changingCharacter(N: Int, K: Int, S: String) -> String {
  let s: [String] = stringToArray(str: S)
  var answer: [String] = []
  
  for i in 0..<s.count {
    if(i == K - 1) {
      answer.append(s[i].lowercased())
    } else {
      answer.append(s[i])
    }
  }

  return answer.joined(separator: "")
}

print(changingCharacter(N: 3, K: 1, S: "ABC"))

```

### B-YYMM or MMYY
```Swift

```
