# only-maths

Mathematical implementations of programming functions.

## Contents

- [Round](#round)
- [Round up](#round-up)
- [Round down](#round-down)
- [Round to interval](#round-to-interval)

## Round

> Depends on [Round down](#round-down)

```math
Round(n) = f(n) = RoundDown(n + 0.5)

Round(1.2) = 1
Round(2.8) = 3
```

## Round up

```
RoundUp(n) = f(n) = n + 1 - (n mod 1)

RoundUp(1.2) = 2
RoundUp(2.8) = 3
```

## Round down

```
RoundDown(n) = f(n) = n - (n mod 1)

RoundDown(1.2) = 1
RoundDown(2.8) = 2
```

## Round to interval

> Depends on [Round](#round)

```
RoundInterval(n, i) = f(n, i) = Round(n / i) * i

RoundInterval(1, 5) = 0
RoundInterval(4, 5) = 5
RoundInterval(8, 5) = 10
```
