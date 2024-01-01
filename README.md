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
Round(n) = RoundDown(n + 0.5)
```

```math
\begin{align}
Round(1.2) &= 1 \\
Round(2.8) &= 3
\end{align}
```

## Round up

```math
RoundUp(n) = n + 1 - (n\ \text{mod}\ 1)
```

```math
\begin{align}
RoundUp(1.2) &= 2 \\
RoundUp(2.8) &= 3
\end{align}
```

## Round down

```math
RoundDown(n) = n - (n\ \text{mod}\ 1)
```

```math
\begin{align}
RoundDown(1.2) &= 1 \\
RoundDown(2.8) &= 2
\end{align}
```

## Round to interval

> Depends on [Round](#round)

```math
RoundInterval(n, i) = Round(n / i) * i
```

```math
\begin{align}
RoundInterval(1, 5) &= 0 \\
RoundInterval(4, 5) &= 5 \\
RoundInterval(8, 5) &= 10
\end{align}
```
