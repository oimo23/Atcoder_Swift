### ABC122
[問題ページ](https://atcoder.jp/contests/abc122/tasks)

### A-Double Helix
```Swift
func doubleHelix(b: String) -> String {
  var answer: String = ""
  
  if b == "A" {
    answer = "T"
  } else if b == "T" {
    answer = "A"
  } else if b == "C" {
    answer = "G"
  } else if b == "G" {
    answer = "C"
  }

  return answer
}

print(doubleHelix(b: "G"))

```

### B-ATCoder
```Swift
// 文字列をそのまま1文字づつ配列にする
func stringToArray(str: String) -> [String] {
  var array: [String] = []

  for s in str {
    array.append(String(s))
  }
  
  return array
}

func aTCoder(S: String) -> Int {
  let s: [String] = stringToArray(str: S)
  var streak: [Int] = [];
  var temp: Int = 0

  for i in 0..<s.count {
    if s[i] != "A", s[i] != "T", s[i] != "C", s[i] != "G" {
      streak.append(temp)
      temp = 0
    } else {
      temp += 1
    }
  }

  if temp != 0 {
    streak.append(temp)
  }

  guard let answer = streak.max() else { return 0 }

  return answer
}

print(aTCoder(S: "ATCODER"))

```
