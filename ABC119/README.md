### ABC119
[問題ページ](https://atcoder.jp/contests/abc119/tasks)

### A-Still TBD
```Swift
func stillTBD(S: String) -> String {
  let s = S.components(separatedBy: "/")
  var answer = "TBD"

  if let unwrapped = Int(s.joined(separator: "")) {
    if unwrapped <= 20190431 {
      answer = "Heisei"
    }
  }

  return answer
}

print(stillTBD(S: "2019/05/01"))

```

### B-Digital Gifts
```Swift
func digitalGifts(N: Int, X: [[String]]) -> Double {
  var total: Double = 0

  for i in 0..<X.count {
    var money: Double = 0
    guard let price: Double = Double(X[i][0]) else { break }

    if X[i][1] == "BTC" {
      money = price * 380000.0
    } else {
      money = price
    }

    total += money
  }

  return total
}

print(digitalGifts(N: 2, X: [["10000", "JPY"], ["0.10000000", "BTC"]]))

```
