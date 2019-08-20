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
func greatOceanView(N: Int, H: [Int]) -> Int {
  var answer: Int  = 1
  var highest: Int = H[0]

  for i in 1..<N {
    if H[i] >= highest {
      answer += 1
    }

    if H[i] > highest {
      highest = H[i]
    }
  }

  return answer
}

print(greatOceanView(N: 4, H: [6, 5, 6, 8]))

```
