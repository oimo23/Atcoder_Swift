### ABC116
[問題ページ](https://atcoder.jp/contests/abc116/tasks)

### A-Right Triangle
```Swift
func rightTriangle(AB: Int, BC: Int, CA:Int) -> Int {
  let sides: [Int] = [AB, BC, CA].sorted{$0 < $1}

  return (sides[0] * sides[1]) / 2
}

print(rightTriangle(AB: 45, BC: 28, CA: 53))

```

### B-Collatz Problem
```Swift

```
