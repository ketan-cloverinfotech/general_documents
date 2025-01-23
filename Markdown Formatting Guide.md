

Table of Contents
-----------------

1.  [Headings](#headings)
2.  [Emphasis](#emphasis)
3.  [Lists](#lists)
    *   [Unordered Lists](#unordered-lists)
    *   [Ordered Lists](#ordered-lists)
    *   [Nested Lists](#nested-lists)
4.  [Links](#links)
5.  [Images](#images)
6.  [Code](#code)
    *   [Inline Code](#inline-code)
    *   [Code Blocks](#code-blocks)
7.  [Blockquotes](#blockquotes)
8.  [Horizontal Rules](#horizontal-rules)
9.  [Tables](#tables)
10.  [Task Lists](#task-lists)
11.  [Strikethrough](#strikethrough)
12.  [Escaping Characters](#escaping-characters)
13.  [Extended Syntax](#extended-syntax)
    *   [Footnotes](#footnotes)
    *   [Definition Lists](#definition-lists)
    *   [Superscript and Subscript](#superscript-and-subscript)
    *   [Highlighting](#highlighting)
    *   [Emoji](#emoji)

* * *

Headings
--------

Headings are created using the `#` symbol. The number of `#` symbols indicates the level of the heading.

```markdown
# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading
```

**Rendered:**

H1 Heading
==========

H2 Heading
----------

### H3 Heading

#### H4 Heading

##### H5 Heading

###### H6 Heading

* * *

Emphasis
--------

You can emphasize text using **bold**, _italic_, _**bold italic**_, and ~strikethrough~.

```markdown
**Bold Text**
*Italic Text*
***Bold Italic Text***
~~Strikethrough Text~~
```

**Rendered:**

**Bold Text**  
_Italic Text_  
_**Bold Italic Text**_  
~Strikethrough Text~

* * *

Lists
-----

### Unordered Lists

Use `-`, `*`, or `+` to create unordered lists.

```markdown
- Item 1
- Item 2
  - Subitem 2.1
  - Subitem 2.2
* Item 3
+ Item 4
```

**Rendered:**

*   Item 1
*   Item 2
    *   Subitem 2.1
    *   Subitem 2.2

*   Item 3

*   Item 4

### Ordered Lists

Use numbers followed by a period to create ordered lists.

```markdown
1. First item
2. Second item
   1. Subitem 2.1
   2. Subitem 2.2
3. Third item
```

**Rendered:**

1.  First item
2.  Second item
    1.  Subitem 2.1
    2.  Subitem 2.2
3.  Third item

### Nested Lists

You can nest lists by indenting them with spaces or tabs.

```markdown
- Item 1
  - Subitem 1.1
    - Subitem 1.1.1
- Item 2
  1. Subitem 2.1
  2. Subitem 2.2
```

**Rendered:**

*   Item 1
    *   Subitem 1.1
        *   Subitem 1.1.1
*   Item 2
    1.  Subitem 2.1
    2.  Subitem 2.2

* * *

Links
-----

Create links using `[link text](URL)` syntax. You can also add a title that appears on hover.

```markdown
[OpenAI](https://www.openai.com)
[OpenAI](https://www.openai.com "OpenAI's Website")
```

**Rendered:**

[OpenAI](https://www.openai.com)  
[OpenAI](https://www.openai.com "OpenAI's Website")

### Automatic Links

You can create automatic links by enclosing the URL in angle brackets.

```markdown
<https://www.example.com>
```

**Rendered:**

[https://www.example.com](https://www.example.com)

* * *

Images
------

Similar to links, but with an exclamation mark `!` before the square brackets.

```markdown
![Alt Text](https://www.example.com/image.jpg)
![Alt Text](https://www.example.com/image.jpg "Image Title")
```

**Rendered:**

  

* * *

Code
----

### Inline Code

Use backticks `` ` `` to denote inline code.

```markdown
Here is some `inline code`.
```

**Rendered:**

Here is some `inline code`.

### Code Blocks

Use triple backticks \`\`\` or indent with four spaces to create code blocks. You can also specify the language for syntax highlighting.

<details> <summary>Click to expand code block examples</summary>

````markdown
```javascript
function greet(name) {
  console.log(`Hello, ${name}!`);
}
````

````python

```markdown
    def greet(name):
        print(f"Hello, {name}!")
````

</details>

**Rendered:**

```javascript
function greet(name) {
  console.log(`Hello, ${name}!`);
}
```

```python
def greet(name):
    print(f"Hello, {name}!")
```

* * *

Blockquotes
-----------

Use `>` to create blockquotes. You can nest blockquotes by adding additional `>` symbols.

```markdown
> This is a blockquote.
>
> > Nested blockquote.
```

**Rendered:**

> This is a blockquote.
> 
> > Nested blockquote.

* * *

Horizontal Rules
----------------

Create horizontal lines using three or more `-`, `*`, or `_`.

```markdown
---
***
___
```

**Rendered:**

* * *

* * *

* * *

* * *

Tables
------

Create tables using pipes `|` and hyphens `-`. You can align columns using colons `:`.

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|:-------:|--------:|
| Left     | Center  | Right   |
| Data 1   | Data 2  | Data 3  |
```

**Rendered:**

| Header 1 | Header 2 | Header 3 |
| --- | --- | --- |
| Left | Center | Right |
| Data 1 | Data 2 | Data 3 |

* * *

Task Lists
----------

Create task lists using `- [ ]` for incomplete and `- [x]` for completed items.

```markdown
- [ ] Task 1
- [x] Task 2
  - [ ] Subtask 2.1
  - [x] Subtask 2.2
```

**Rendered:**

*   [ ]  Task 1
*   [x]  Task 2
    *   [ ]  Subtask 2.1
    *   [x]  Subtask 2.2

* * *

Strikethrough
-------------

Use `~~` to strikethrough text.

```markdown
This is ~~strikethrough~~ text.
```

**Rendered:**

This is ~strikethrough~ text.

* * *

Escaping Characters
-------------------

Use a backslash `\` to escape Markdown characters if you want to display them as plain text.

```markdown
\*This text is not italicized\*
```

**Rendered:**

\*This text is not italicized\*

* * *

Extended Syntax
---------------

### Footnotes

Add footnotes using `[^1]` in the text and defining them elsewhere.

```markdown
This is a sentence with a footnote.[^1]

[^1]: This is the footnote.
```

**Rendered:**

This is a sentence with a footnote.[1](#user-content-fn-1)

### Definition Lists

Define terms using a colon `:`.

```markdown
Term 1
: Definition for term 1.

Term 2
: Definition for term 2.
```

**Rendered:**

Term 1 : Definition for term 1.

Term 2 : Definition for term 2.

### Superscript and Subscript

Use `^` for superscript and `~` for subscript.

```markdown
E = mc^2^  
H~2~O
```

**Rendered:**

E = mc²  
H₂O

### Highlighting

Highlight text using double equals `==`.

```markdown
This is ==highlighted== text.
```

**Rendered:**

This is ==highlighted== text.

### Emoji

Use `:` to include emojis.

```markdown
I love programming! :heart: :+1:
```

**Rendered:**

I love programming! ❤️ 👍

* * *

Complete Example
----------------

Here's a complete Markdown example incorporating various elements discussed above:

````markdown
# Project Title

## Introduction

Welcome to the **Project Title**! This project aims to solve the following problems:

- Improve efficiency
- Enhance user experience
- Increase scalability

### Features

1. User Authentication
2. Real-time Data Processing
   - Streaming capabilities
   - Data visualization
3. Reporting Tools

## Usage

To get started, clone the repository:

```bash
git clone https://github.com/username/project.git
````

Then install the dependencies:

```bash
npm install
```

Contributing
------------

Contributions are welcome! Please follow these steps:

*   Fork the repository
*   Create a new branch (`git checkout -b feature/YourFeature`)
*   Commit your changes (`git commit -m "Add YourFeature"`)
*   Push to the branch (`git push origin feature/YourFeature`)
*   Open a pull request

License
-------

This project is licensed under the MIT License.

Contact
-------

For questions or feedback, reach out to email@example.com.

````markdown

**Rendered:**

# Project Title

## Introduction

Welcome to the **Project Title**! This project aims to solve the following problems:

- Improve efficiency
- Enhance user experience
- Increase scalability

### Features

1. User Authentication
2. Real-time Data Processing
   - Streaming capabilities
   - Data visualization
3. Reporting Tools

## Usage

To get started, clone the repository:

```bash
git clone https://github.com/username/project.git
````

Then install the dependencies:

```bash
npm install
```

Contributing
------------

Contributions are welcome! Please follow these steps:

*   Fork the repository
*   Create a new branch (`git checkout -b feature/YourFeature`)
*   Commit your changes (`git commit -m "Add YourFeature"`)
*   Push to the branch (`git push origin feature/YourFeature`)
*   Open a pull request

License
-------

This project is licensed under the MIT License.

Contact
-------

For questions or feedback, reach out to email@example.com.

* * *

This comprehensive guide should cover most of the Markdown formatting options you need. Remember that different platforms might support additional or slightly different syntax extensions, so it's always a good idea to check the specific Markdown documentation for the platform you're using.
