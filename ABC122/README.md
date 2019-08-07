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

```
