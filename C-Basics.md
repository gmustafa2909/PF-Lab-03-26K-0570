# C Basics

## 1. Data Types

| Data Type | Description                                     |
| --------- | ----------------------------------------------- |
| `int`     | Stores whole numbers without decimal values.    |
| `float`   | Stores single-precision floating-point numbers. |
| `double`  | Stores double-precision floating-point numbers. |
| `char`    | Stores a single character.                      |
| `bool`    | Stores a Boolean value: true or false.          |
| `void`    | Represents the absence of a value or data type. |

## 2. Format Specifiers

| Format Specifier | Description                                                    |
| ---------------- | -------------------------------------------------------------- |
| `%d`             | Used to display a signed decimal integer.                      |
| `%u`             | Used to display an unsigned decimal integer.                   |
| `%o`             | Used to display an integer in octal format.                    |
| `%x`             | Used to display an integer in lowercase hexadecimal format.    |
| `%X`             | Used to display an integer in uppercase hexadecimal format.    |
| `%f`             | Used to display a floating-point value in decimal notation.    |
| `%e`             | Used to display a floating-point value in scientific notation. |
| `%c`             | Used to display a single character.                            |
| `%s`             | Used to display a string.                                      |
| `%ld`            | Used to display a long integer.                                |

## 3. Input/Output Functions

### scanf()

`scanf()` is used to take formatted input from the user.

Example:

```c
scanf("%d", &age);
```

### printf()

`printf()` is used to display formatted output on the screen.

Example:

```c
printf("Age = %d", age);
```

### getchar()

`getchar()` reads a single character from the keyboard.

Example:

```c
char ch;
ch = getchar();
```

### putchar()

`putchar()` displays a single character on the screen.

Example:

```c
putchar(ch);
```

### fgets()

`fgets()` is used to read a line of text, including spaces.

Example:

```c
fgets(name, 50, stdin);
```

### puts()

`puts()` displays a string followed by a newline.

Example:

```c
puts(name);
```

## 4. Escape Sequences

Escape sequences are special character combinations used inside C strings and character constants.

| Escape Sequence | Meaning               | Example                        |
| --------------- | --------------------- | ------------------------------ |
| `\n`            | New line              | `printf("Hello\nWorld");`      |
| `\t`            | Horizontal tab        | `printf("Name\tAge");`         |
| `\\`            | Backslash             | `printf("C:\\Files");`         |
| `\"`            | Double quotation mark | `printf("He said \"Hello\"");` |
| `\'`            | Single quotation mark | `printf("It\'s C");`           |
| `\b`            | Backspace             | `printf("ABC\b");`             |
| `\r`            | Carriage return       | `printf("Hello\r");`           |

## 5. Precision

Precision specifies the number of digits displayed after the decimal point for floating-point output.

In `printf()`, precision is specified using a dot followed by the required number of digits.

For example:

```c
printf("%.2f", number);
```

This displays the floating-point value with **2 digits after the decimal point**.

Other examples:

```c
printf("%.3f", number);
printf("%.4f", number);
printf("%.6f", number);
```

For example, if:

```c
float number = 12.345678;
```

then:

```c
printf("%.2f", number);
```

displays:

```text
12.35
```
