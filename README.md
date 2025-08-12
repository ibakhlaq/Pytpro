<p align="center">
  <img src="https://i.postimg.cc/BjSmyvYv/download.png" width="200" alt="pytpro logo">
</p>

<p align="center">
  <img src="https://i.postimg.cc/s2PM4pyd/pyt.png" width="140" alt="pytpro heading">
</p>

**pytpro** is a lightweight Python package by Ibrahim Akhlaq that provides powerful utility functions for math, randomness, and HTML rendering. It's clean, minimal, and built to feel like magic.
---

# 🖥️ Example Usage

```python
import pytpro

pytpro.add(2, 3)
pytpro.square(6)
pytpro.pi()
pytpro.htmlcssjs("<h1>Hello!</h1><p>This is raw HTML.</p>")
```

# 🖥️ Instructions to install:

To install locally from your project directory, open PowerShell or terminal and run:

```bash
pip install pytpro
```

# API REFERENCE

- disclaimer: Some of the output examples in the API reference cannot be rendered in PYPI, so screenshots of the actual results were provided. Keep in mind that the output may differ slightly from the actual results, as I had to resize the images in some cases.

---

## 🚀 Features
### ➕ Math Functions:
- `add(a, b):`

The _`add()`_ function takes two numbers __`a`__ and __`b`__ and returns their sum.

- `subtract(a, b):`

The _`subtract()`_ function takes two numbers __`a`__ and __`b`__ and returns their difference __`a`-`b`__.
- `multiply(a, b):`

The _`multiply()`_ function takes two numbers __`a`__ and __`b`__ and returns their product.
- `divide(a, b):`

The _`divide()`_ function takes two numbers __`a`__ and __`b`__ and returns their quotient __`a`/`b`__.
- `modulus(a, b):`

The _`modulus()`_ function takes two numbers __`a`__ and __`b`__ and returns the remainder of __`a`/`b`__.
- `floordivision(a, b):`

The _`floordivision()`_ function takes two numbers __`a`__ and __`b`__ and returns the largest integer less than or equal to __`a`/`b`__.
- `square(a)` / `cube(a):`

These functions return the square or cube (respectively) of a number __`a`__.
- `squareroot(a)` / `cuberoot(a):`

These functions return the square root or cube root (respectively) of a number __`a`__.
- `absolutevalue(a):`

The _`absolutevalue()`_ function returns the absolute value of a number __`a`__.
- `roundoff(a):`

The _`roundoff()`_ function rounds a number __`a`__ to the nearest integer.
- `exponent(a, b)` / `power(a, b)`

These functions return __`a`__ raised to the power of __`b`__.They are the same functions but they have different names for convenience.

### 🔢 Random Number Generators
- `randint(start=0, end=100):`

The _`randint()`_ function generates a random integer between __`start`__ and __`end`__ (inclusive). The default value is 0 to 100.
- `randfloat():`

This function (_`randfloat()`_) generates a random floating-point number between 0 and 1. It requires no parameters or arguments, and if you want to generate a random float in a specific range, you can use the _`randomfloatpositive(start, end)`_ or *`randomfloatnegative(start, end)`* functions. Inputting an argument or parameter could result in errors.
- `randomintpositive(start, end, step=1):`

The function _`randomintpositive()`_ generates a random integer between __`start`__ and __`end`__ (inclusive) with a step size of __`step`__.
The return value of this function will always be a positive value, whether the input is positive or negative.
- `randomintnegative(start, end, step=1):`

The function _`randomintnegative()`_ generates a random integer between __`start`__ and __`end`__ (inclusive) with a step size of __`step`__.
The only difference between this function and the _`randomintpositive()`_ function is that the generated integer will return a negative value, whether the input is positive or negative.
- `randomfloatpositive(start, end):`

The function _`randomfloatpositive()`_ generates a random floating-point number between __`start`__ and __`end`__ (inclusive). Just like the _`randomintpositive()`_ function, the return value of this function will always be a positive value, whether the input is positive or negative.
- `randomfloatnegative(start, end):`

The function _`randomfloatnegative()`_ generates a random floating-point number between __`start`__ and __`end`__ (inclusive). Just like the _`randomintnegative()`_ function, the return value of this function will always be a negative value, whether the input is positive or negative.
- `randomfloat(start, end):`

The function _`randomfloat()`_ generates a random floating-point number between __`start`__ and __`end`__ (inclusive).

### 📐 Trigonometry & Logs
```javascript
(1) sine(x)
(2) cosine(x)
(3) tangent(x)
(4) arctangent(x)
(5) log_base_2(x)
(6) log_base_10(x)
(7) natural_log(x)
```
The functions above return the sine, cosine, tangent, arctangent, log base 2, log base 10, and natural logarithm of a number __*`x`*__ respectively.

---
### 📏 Constants
```python
`pi()`, `e()`, `goldenratio()`, `tau()`
`speedoflight()`, `planckconstant()`, `gravitationalconstant()`
`electronmass()`, `protonmass()`, `neutronmass()`
`electronvolt()`, `joule()`, `kilojoule()`, `megajoule()`, `gigajoule()`, `terajoule()`, `petajoule()`, `exajoule()`
```
The functions above return the value of their respective constants. Note that the functions have no parameters or arguments. If any parameter or argument is provided, it could result in errors that are extremely hard to diagnose.

---

## HTML RENDERING
### `page_title(text)`
You can use the `page_title()` function to render a title in HTML text.
####     Example
```python
import pytpro as py
py.page_title("Hello World!")
```
#### Output
```HTML
<title>Hello World!</title>
```
### `write(text)`
You can use the `write()` function to render text.
####     Example
```python
import pytpro as py
py.write("Hello World!")
```
#### Output
```HTML
<p>Hello World!</p>
```
- <p>Hello World!</p>


### `title(text)`
You can use the `title()` function to render a title as HTML text.
####     Example
```python
import pytpro as py
py.title("Hello World!")
```
#### Output
```HTML
<h1>Hello World!</h1>
```
- <h1>Hello World!</h1>

### `header(text)`
You can use the `header()` function to render a header as HTML text.
####     Example
```python
import pytpro as py
py.header("Hello World!")
```
#### Output
```HTML
<h2>Hello World!</h2>
```
- <h2>Hello World!</h2>

### `subheader(text)`
You can use the `subheader()` function to render a subheader as HTML text.
####     Example
```python
import pytpro as py
py.subheader("Hello World!")
```
#### Output
```HTML
<h3>Hello World!</h3>
```
- <h3>Hello World!</h3>
### `caption(text)`
You can use the `caption()` function to render a caption as HTML text.
####     Example
```python
import pytpro as py
py.caption("Hello World!")
```
#### Output
```HTML
<p style='font-size: 0.9em; color: gray;'>Hello World!</p>
```
<p align="left"><img src='https://i.postimg.cc/hjRzR2D5/caption.png' width='90' alt='Hello World!'></p>

### `htmlcssjs(html_fragment)`
You can use the `htmlcssjs()` function to render raw HTML, CSS, and Javascript code.
####     Example
```python
import pytpro as py
py.htmlcssjs("""
<style>
button {
    background-color: red;
    border: none;
    border-radius: 4px;
    padding: 15px 32px;
    color: white;
}
</style>
<button onclick='click()'>Hello World!</button>
<p id="output"></p>
<script>
  const output = document.getElementById('output');
  function click() {
    output.innerHTML = 'Hello World!';
  }
</script>
""")
```
#### Output
```HTML
<style>
button {
    background-color: red;
    border: none;
    border-radius: 4px;
    padding: 15px 32px;
    color: white;
}
</style>
<button onclick='click()'>Hello World!</button>
<p id="output"></p>
<script>
  const output = document.getElementById('output');
  function click() {
    output.innerHTML = 'Hello World!';
  }
</script>
```
<p>
<img src="https://i.postimg.cc/NfyFK8rf/pypi2.png" width="230" alt="button">
</p>

### Alert Boxes
#### `alertbox_red(text)`
#### `alertbox_green(text)`
#### `alertbox_blue(text)`
#### `alertbox_yellow(text)`
#### `alertbox_purple(text)`
#### `alertbox_orange(text)`
#### `alertbox_pink(text)`
#### `alertbox_cyan(text)`
#### `alertbox_lime(text)`
#### `alertbox_brown(text)`
#### `alertbox_gray(text)`
#### `alertbox_black(text)`

You can use the `alertbox_*()` functions to display alert boxes. Each function takes a text argument, which is the message to be displayed in the alert box. The alert boxes have different colors and styles, making them visually distinct from each other.

### Example
```python
import pytpro as py
py.alertbox_red("Hello World!")
```
#### Output
```HTML
    <div style='
        padding: 16px;
        margin: 10px 0;
        background-color: #fdecea;
        color: #b00020;
        border-left: 6px solid #b00020;
        border-radius: 4px;
        font-family: sans-serif;
    '>
        Hello World!
    </div>
```

  <p align="left">
  <img src='https://i.postimg.cc/MTQNyRsJ/pypi.png' border='0' alt='pypi'/></a>
  </p>


### Toast Notifications (auto-fade)
- `toast(text, color, duration)` – default color is white, fades after duration seconds (default: 5). Only background color is supported.
- `toast_custom(text, color, text_color, duration)` – custom color, custom text color, fades after 5 seconds(the duration), default text color is black and color is white. HEX, RGB, RGBA, and HSL are supported.

You can use the `toast()` function to display a toast notification with a default color of white. The function takes a text argument, which is the message to be displayed in the toast notification. The toast notification will automatically fade out after 5 seconds unless you provide a custom duration as an argument. The `toast_custom()` function allows you to customize both the background and text color, as well as the fade-out duration.
### Example
```python
import pytpro as py
py.toast("Hello World!")
```
```python
import pytpro as py
py.toast("Hello World!", color="olive", duration=2)
```
<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExaW90N2VhaWVscjBybHpoaWRxaWNmbHhoNjFtaW51Z2JhZjJhamEweCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/cZxJjaszVM981bzM4S/giphy.gif" alt="toast olive" width="46.7%">
  <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExZGgyaDg3bjRlcnFodzBkandvMmhteDRoeTU5c2hlZWdyNW9yZ2g3bCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/4rP0TRhnyZvrrzwdyH/giphy.gif" alt="toast custom" width="45%">
</p>


_The available colors for `toast` are_:                                                                                                                                                                                                                                                                                                             
 **red**, **green**, **blue**, **black**, **pink**, **white**, **yellow**, **orange**, **purple**, **brown**, **gray**, **teal**, **lime**, **indigo**, **cyan**, **magenta**, **olive**, **navy**, _and_ **maroon**.

The only difference between the two functions is that:
- `toast_custom()` allows custom background and text color.
- `toast()` only lets you choose the background color, and the text color adjusts automatically.

---

# Markdown Preview

### `markdown(text)`

You can use the `markdown()` function to display markdown text.

### Example:
```python
import pytpro as py
py.markdown("""
# Hello World!
This is a paragraph with **bold**, *italic*, and `inline code`.
""")
```
```HTML
<h1> Hello World!</h1>
<p>This is a paragraph with <strong>bold</strong>, <em>italic</em>, and <code>inline code</code>.</p>
```
- <h1>Hello World!</h1>
  <p> This is a paragraph with <strong>bold</strong>, <em>italic</em>, and <code>inline code</code>.</p>

For more information about Markdown formatting and its syntax, see the [Markdown documentation](https://www.markdownguide.org/), [cheat sheet](https://www.markdownguide.org/cheat-sheet/), [basic syntax](https://www.markdownguide.org/basic-syntax/), or [extended syntax](https://www.markdownguide.org/extended-syntax/).
---

<h1 align="center">Pytpro</h1>

<pre>
 _______  ___    ___ ________  _______    _________    ________
|   ___  \\  \  /  /|__    __||   ___  \ |   ___   | /  ______  \
|  |___|  |\  \/  /    |  |   |  |___|  ||  |___|  ||  /      \  |
|   _____/  \    /     |  |   |   _____/ |    ____/ |  |      |  |
|  |         \  /      |  |   |  |       |    \___  |  |      |  |
|  |         |  |      |  |   |  |       |  |\__  \_|  \______/  |
|__|         |__|      |__|   |__|       |__|   \____\ ________ /
</pre>

__version:0.3.0__