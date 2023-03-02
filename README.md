# 🎨 Colorway

Python package to change the text color of the python console.  

## 📦 Installation

Run the following to install:  

```bash
$ pip install colorway
```

## 🚀 Usage

### Foreground

```python
from colorway_foreground import *

# Generate red text with default background
print(red_fg("Hello, World!"))

# Generate bold red text with default background
print(bold_red_fg("Hello, World!"))

# Generate high-intensity red text with default background
print(highintensity_red_fg("Hello, World!"))

# Generate high-intensity bold red text with default background
print(highintensity_bold_red_fg("Hello, World!"))

# Generate custom colored text (red: 150, green: 78, blue: 120) with default background
print(custom_fg(150,78,120,"Hello, World!"))
```

### Background

```python
from colorway_background import *

# Generate text with red background
print(red_bg("Hello, World!"))

# Generate text with high-intensity red background
print(highintensity_red_bg("Hello, World!"))

# Generate text with custom colored background (red: 150, green: 78, blue: 120)
print(custom_bg(150,78,120,"Hello, World!"))
```

### Foreground & Background

You can use foreground formatting and background formatting by placing them in each other.  

```python
from colorway_foreground import *
from colorway_background import *

# Generate red text with blue background
print(red_fg(blue_bg("Hello, World!")))
```

### Manual

You can also use the manual package to manually format parts of strings.

```python
from colorway_manual import *

# Generate red text
print(f'{foreground.red}Hello, World!{format.clear}')

# Generate text with red background
print(f'{background.red}Hello, World!{format.clear}')

# Generate text with a mix of colors
print(f'{foreground.red}Hello, {background.blue}World!{format.clear}')
```

### Available colors
#### Foreground
- `black_fg(string)`
- `red_fg(string)`
- `green_fg(string)`
- `yellow_fg(string)`
- `blue_fg(string)`
- `purple_fg(string)`
- `cyan_fg(string)`
- `white_fg(string)`
- `bold_black_fg(string)`
- `bold_red_fg(string)`
- `bold_green_fg(string)`
- `bold_yellow_fg(string)`
- `bold_blue_fg(string)`
- `bold_purple_fg(string)`
- `bold_cyan_fg(string)`
- `bold_white_fg(string)`
- `underline_black_fg(string)`
- `underline_red_fg(string)`
- `underline_green_fg(string)`
- `underline_yellow_fg(string)`
- `underline_blue_fg(string)`
- `underline_purple_fg(string)`
- `underline_cyan_fg(string)`
- `underline_white_fg(string)`
- `highintensity_black_fg(string)`
- `highintensity_red_fg(string)`
- `highintensity_green_fg(string)`
- `highintensity_yellow_fg(string)`
- `highintensity_blue_fg(string)`
- `highintensity_purple_fg(string)`
- `highintensity_cyan_fg(string)`
- `highintensity_white_fg(string)`
- `highintensity_bold_black_fg(string)`
- `highintensity_bold_red_fg(string)`
- `highintensity_bold_green_fg(string)`
- `highintensity_bold_yellow_fg(string)`
- `highintensity_bold_blue_fg(string)`
- `highintensity_bold_purple_fg(string)`
- `highintensity_bold_cyan_fg(string)`
- `highintensity_bold_white_fg(string)`
- `custom_fg(red, green, blue, string)`

#### Background
- `black_bg(string)`
- `red_bg(string)`
- `green_bg(string)`
- `yellow_bg(string)`
- `blue_bg(string)`
- `purple_bg(string)`
- `cyan_bg(string)`
- `white_bg(string)`
- `highintensity_black_bg(string)`
- `highintensity_red_bg(string)`
- `highintensity_green_bg(string)`
- `highintensity_yellow_bg(string)`
- `highintensity_blue_bg(string)`
- `highintensity_purple_bg(string)`
- `highintensity_cyan_bg(string)`
- `highintensity_white_bg(string)`
- `custom_bg(red, green, blue, string)`

#### Manual
- `format.clear`
- `foreground.black`
- `foreground.red`
- `foreground.green`
- `foreground.yellow`
- `foreground.blue`
- `foreground.purple`
- `foreground.cyan`
- `foreground.white`
- `foreground.bold.black`
- `foreground.bold.red`
- `foreground.bold.green`
- `foreground.bold.yellow`
- `foreground.bold.blue`
- `foreground.bold.purple`
- `foreground.bold.cyan`
- `foreground.bold.white`
- `foreground.underline.black`
- `foreground.underline.red`
- `foreground.underline.green`
- `foreground.underline.yellow`
- `foreground.underline.blue`
- `foreground.underline.purple`
- `foreground.underline.cyan`
- `foreground.underline.white`
- `foreground.highintensity.black`
- `foreground.highintensity.red`
- `foreground.highintensity.green`
- `foreground.highintensity.yellow`
- `foreground.highintensity.blue`
- `foreground.highintensity.purple`
- `foreground.highintensity.cyan`
- `foreground.highintensity.white`
- `foreground.highintensity.bold.black`
- `foreground.highintensity.bold.red`
- `foreground.highintensity.bold.green`
- `foreground.highintensity.bold.yellow`
- `foreground.highintensity.bold.blue`
- `foreground.highintensity.bold.purple`
- `foreground.highintensity.bold.cyan`
- `foreground.highintensity.bold.white`
- `foreground.custom(red, green, blue)`
- `background.black`
- `background.red`
- `background.green`
- `background.yellow`
- `background.blue`
- `background.purple`
- `background.cyan`
- `background.white`
- `background.highintensity.black`
- `background.highintensity.red`
- `background.highintensity.green`
- `background.highintensity.yellow`
- `background.highintensity.blue`
- `background.highintensity.purple`
- `background.highintensity.cyan`
- `background.highintensity.white`
- `background.custom(red, green, blue)`

### Note
Please be aware that you can **not** combine foreground and background formatting if you use high-intensity colors.  
Please be aware that custom colors may **not** be supported by all terminal outputs.  

## 👨‍💻 Developing Colorway

To install colorway, along with the tools you need to develop and run tests, run the following in your virtualenv:

```bash
$ pip install -e .[dev]
```

## 🚦 Development Progress

Stable Development 
