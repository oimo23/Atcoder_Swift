### ABC114
[問題ページ](https://atcoder.jp/contests/abc114/tasks)

### A-753
```Swift
func sevenFiveThree(X: Int) -> String {
  return X == 7 || X == 5 || X == 3 ? "YES" : "NO"
}

print(sevenFiveThree(X: 3))

```

### B-754
```Swift
// 文字列をそのまま1文字づつ配列にする
func stringToArray(str: String) -> [String] {
  var array: [String] = []

  for s in str {
    array.append(String(s))
  }
  
  return array
}

func sevenFiveFour(S: String) -> Int {
  var diffs: [Int] = []
  var num: [String] = stringToArray(str: S)

  for i in 0..<S.count-3 {
    let temp: Int = Int(num[i..<(i+3)].joined(separator: "")) ?? 0
    diffs.append(abs(753 - temp))
  }

  guard let answer: Int = diffs.min() else { return 0 }

  return answer
}

print(sevenFiveFour(S: "1234567876"))

```
