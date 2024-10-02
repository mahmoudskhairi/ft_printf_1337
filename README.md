# ft_printf Project

<!-- HTML for the image (replace with an actual path or URL) -->
<img src="printf_2.png" alt="Libft Logo" style="max-width: 100%; height: auto;">

## Project Overview

<p>
The **ft_printf** project is a custom implementation of the C standard library function <code>printf</code>. The goal is to deepen the understanding of formatted output functions in C and enhance skills in handling variable arguments and format specifiers.
</p>

## Features

<ul>
  <li>Supports a variety of format specifiers: <code>%c, %s, %d, %i, %u, %x, %X, %p, %% </code>.</li>
  <li>Handles flags for formatting such as <code>-</code>, <code>+</code>, <code>0</code>, and width specifiers.</li>
  <li>Implements precision for decimal, strings, and hexadecimal outputs.</li>
</ul>

## Installation

<p>To install and run this project:</p>

<pre>
  git clone https://github.com/mahmoudskhairi/ft_printf_42.git
  cd ft_printf
  make
</pre>

## Usage

<p>Here's an example of how to use the <code>ft_printf</code> function:</p>

<pre>
#include "ft_printf.h"

int main() {
    int number = 42;
    char *str = "Hello, World!";
    
    ft_printf("Number: %d\nString: %s\n", number, str);
    return 0;
}
</pre>

<h2 id="contact">Contact</h2>
<p>For any questions, feedback, or issues, feel free to reach out:</p>
<ul>
  <li>Email: <a href="mailto:mahmoud.skhairi@gmail.com">mahmoud.skhairi@gmail.com</a></li>
  <li>LinkedIn: <a href="https://www.linkedin.com/in/mahmoud-skhairi" target="_blank">mahmoud skhairi</a></li>
</ul>

<h2>Happy Coding!</h2>
