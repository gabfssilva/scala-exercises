# scala-exercises
A few exercises to help people get started with Scala, OO and FP. ;)

#### Note: this is still under development.

## 1 - Basic types


| Type    | Description                                                      |
|---------|------------------------------------------------------------------|
| Byte    | 8 bit signed value. Range from -128 to 127                       |
| Short   | 16 bit signed value. Range -32768 to 32767                       |
| Int     | 32 bit signed value. Range -2147483648 to 2147483647             |
| Long    | 64 bit signed value. -9223372036854775808 to 9223372036854775807 |
| Float   | 32 bit IEEE 754 single-precision float                           |
| Double  | 64 bit IEEE 754 double-precision float                           |
| Char    | 16 bit unsigned Unicode character. Range from U+0000 to U+FFFF   |
| String  | A sequence of Chars                                              |
| Boolean | Either the literal true or the literal false                     |

## 2 - Declaring values

In Scala, basically you have two ways to declare a value: using `var` or `val`.

Th difference between them is that `var` is mutable and `val` is not.

E.g.:

```scala
//You can do that
var x = 2
x = 4

//But NOT that
val y = 2
y = 4 //does not compile
```

Since Scala has type inference, you don't have to inform which type a value is, but, you can inform explicitly if you want to:

```scala
val x: Int = 2
```

Scala does not allow you to reassigned a value using a different type that you first assigned.

```scala
var x: Int = 2
x = "a string" //does not compile

var y = "another string"
y = 2 //does not compile
```

## Conditional statements

You can use conditional statements in Scala using `if`, `else if` and `else`.

```scala
val x = 2

if (x == 2) {
  println("x value is 2")
} else if (x == 3) {
  println("x value is 3")
} else {
  println("x value is " + x)
}

```
