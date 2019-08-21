### ABC087
[問題ページ](https://atcoder.jp/contests/abc087/tasks)

### A-Buying Sweets
```Swift
func buyingSweets(X: Int, A: Int, B: Int) -> Int {
  return (X - A) % B
}

print(buyingSweets(X: 1234, A: 150, B: 100))

```

### B-Coins
```Swift
func coins(A: Int, B: Int, C: Int, X: Int) -> Int {
  var cnt: Int = 0

  //　全探索する
  for i in 0...A {
    for j in 0...B {
      for k in 0...C {
        let sum = (500 * i) + (100 * j) + (50 * k);
        
        if sum == X {
          cnt += 1
        }
      }
    }
  }

  return cnt
}

print(coins(A: 30, B: 40, C: 50, X: 6000))

```