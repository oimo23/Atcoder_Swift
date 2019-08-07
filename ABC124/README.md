### ABC124
[問題ページ](https://atcoder.jp/contests/abc124/tasks)

### A-Buttons
```Swift
func buttons(A: Int, B: Int) -> Int {
  var answer: Int = 0

  if (A - B) == 0 {
    answer = A + B
  }  else {
    answer = (max(A, B) * 2) - 1
  }

  return answer
}

print(buttons(A: 3, B: 3))

```

### B-Great Ocean View
```Swift

```
