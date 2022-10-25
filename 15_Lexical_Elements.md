## 15.5 抽象字面量

### 15.5.1 概括

有两类抽象字面量：实数型字面量和整型字面量。一个实数型字面量是包含符号“点”的抽象字面量；一个整型字面量是不包含符号“点”的抽象字面量。实数字面量拥有字面量类型*universal_real*，整型字面量拥有字面量类型*universal_integer*

```
abstract_literal ::= decimal_literal | based_literal
```

### 15.5.2 十进制字面量

一个十进制字面量是一类可以转换为十进制（即满十进一）表示的抽象字面量

```
decimal_literal ::= integer[.integer][exponent]
integer ::= {[underline]digit}
exponet ::= E[+]integer|E-integer
```
