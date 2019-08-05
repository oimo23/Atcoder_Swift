### ABC081
[問題ページ](https://atcoder.jp/contests/abc081/tasks)

### A-Placing Marbles
```Swift
func placingMarbles(S: String) -> Int {
  var cnt: Int = 0

  for s in S {
    if s == "1" {
      cnt += 1
    }
  }

  return cnt;
}

print(placingMarbles(S: "1011"))

```

### B-Shift Only
```Swift
func shiftOnly(N: Int, A: [Int]) -> Int {
  var numbers: [Int] = A
  var cnt: Int  = 0
  var flg: Bool = true

  while flg {
    for i in 0..<N {
      if(numbers[i] % 2 == 0) {
        numbers[i] /= 2;
      } else {
        flg = false
        break
      }
    }

    if flg {
      cnt += 1
    }
  }

  return cnt
}

print(shiftOnly(N: 3, A:[8, 12, 40]))

```