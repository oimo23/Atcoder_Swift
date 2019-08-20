### ABC123
[問題ページ](https://atcoder.jp/contests/abc123/tasks)

### A-Five Antennas
```Swift
func fiveAntennas(a: Int, b: Int, c: Int, d: Int, e: Int, k: Int) -> String {
  return e - a > k ? ":(" : "Yay!"
}

print(fiveAntennas(a: 1, b: 2, c: 4, d: 8, e: 9, k: 15))

```

### B-Five Dishes
```Swift
func fiveDishes(times: [Int]) -> Int {
  var min: Int = 10
  var sum: Int = 0

  for i in 0..<5 {
    let digitOne: Int = times[i] % 10
    sum += times[i]

    if 10 - digitOne != 10 {
      sum += 10 - digitOne
    }

    if 10 - digitOne != 10 && digitOne < min {
      min = digitOne
    }
  }

  return sum - (10 - min)
}

print(fiveDishes(times: [29, 20, 7, 35, 120]))

```
