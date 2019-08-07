### ABC119
[問題ページ](https://atcoder.jp/contests/abc119/tasks)

### A-Still TBD
```JavaScript
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
```JavaScript

```
