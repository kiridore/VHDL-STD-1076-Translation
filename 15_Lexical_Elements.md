## 15.5 抽象字面量 (Abstract literals)

### 15.5.1 概括 (General)

有两类抽象字面量：实数型字面量和整型字面量。一个实数型字面量是包含符号“点”的抽象字面量；一个整型字面量是不包含符号“点”的抽象字面量。实数字面量拥有字面量类型*universal_real*，整型字面量拥有字面量类型*universal_integer*

```
abstract_literal ::= decimal_literal | based_literal
```

### 15.5.2 十进制字面量 (Decimal literals)

一个十进制字面量是一类可以转换为十进制（即满十进一）表示的抽象字面量

```
decimal_literal ::= integer[.integer][exponent]
integer ::= {[underline]digit}
exponet ::= E[+]integer|E-integer
```

插入在十进制字面量中两个数字之间的下划线字符不会影响该抽象字面量的值。上述生成式*exponent*中的字母E可以任意使用大写或小写，不会影响其含义。


An exponent indicates the power of 10 by which the value of the decimal literal without the exponent is to be multiplied to obtain the value of the decimal literal with the exponent.一个整型字面量的幂次不应该包含负号。