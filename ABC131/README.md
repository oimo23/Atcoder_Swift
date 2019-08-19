### ABC131
[問題ページ](https://atcoder.jp/contests/abc131/tasks)

### A-Security
```Swift
func stringToArray(str: String) -> [String] {
  var array: [String] = []

  for s in str {
    array.append(String(s))
  }
  
  return array
}

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
func biteEating(N: Int, L: Int) -> Int {
  var list: [Int] = []

  for i in 0..<N {
    let taste: Int = (L + i + 1) - 1

    list.append(taste)
  }

  let max: Int = list.reduce(0){(m,n) -> Int in m + n}
  var min: Int = 10000000
  var target: Int = 0

  for i in 0..<N {
    let temp: Int = max - list[i]
    let absValue: Int  = abs(max - temp)

    if absValue < min {
      min = absValue
      target = i
    }
  }

  list.remove(at: target)

  return list.reduce(0){(m,n) -> Int in m + n}
}

print(biteEating(N: 5, L: 2))

```