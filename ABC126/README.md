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
func yymmOrMmyy(S: String) -> String {
  guard let first: Int = Int(String(S.prefix(2))) else { return "error"}
  guard let last:  Int = Int(String(S.suffix(2))) else { return "error"}

  // 両方1 ~ 12
  if(
    first > 0 && 12 >= first &&
    last  > 0 && 12 >= last
  ) {
    return "AMBIGUOUS"
  }

  // YYMMのみ有りえる
  if(
    first <= 0 || 12 < first &&
    last  >  0 && 12 >= last
  ) {
    return "YYMM"
  }

  // MMYYのみ有りえる
  if(
    first > 0 && 12 >= first &&
    last  > 0 && 12 >= last
  ) {
    return "MMYY"
  }

  return "NA"
}

print(yymmOrMmyy(S: "1905"))

```
