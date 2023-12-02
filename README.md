# Markdown Tutorial
### Author: Madeline Prater
This is a tutorial meant to teach about the various things that can be done in Markdown, and how to do each of them, with examples.

If you are interested in using Markdown and want an overview of the various things that can be done with it, this tutorial is intended for you.

---

### Table of Contents

[Escape Character](#escape-character)  
[Basic Formatting](#basic-formatting)  
[Headers](#headers)  
[Line Spacing and Breaks](#line-spacing-and-breaks)  
[Lists, Quotes, and Code Blocks](#lists-quotes-and-code-blocks)  
[Links](#links)  
[Tables](#tables)  

---

## Escape Character

The first thing to understand about Markdown is the escape character, which is the backslash ( \\ ).  
Many characters are used by Markdown for formatting, and attempting to put them into a page will instead use them for that formatting, causing them to not appear.  
An escape character is used whenever you want the next character after it to remain visible and not be used for any Markdown formatting.

For example, the pound key ( \# ) is used for headers. In order to have it display in text without creating a header, it must be preceded by a backslash.  
Inputting the following line   
```
\# Hello World
```
Will result in the following text being displayed:

\# Hello World

Without the backslash, it will instead look like this:

# Hello World

Any time you see a Markdown formatting character written normally in this guide, it's been done using a backslash preceding it.

---

## Basic Formatting

There are many simple things that can be done in markdown. The asterisk ( \* ) character is used for Italic, Bold, and Bold Italic text.

Surrounding text with a single asterisk gives italic text, like so:

```
*Hello World*
```

*Hello World*

Surrounding it with two asterisks instead gives bold text:

```
**Hello World**
```

**Hello World**

And using three asterisks results in bold italic text:

```
***Hello World***
```

***Hello World***

Additionally, you can strikethrough text by surrounding the text with two tilde ( \~\~ ) on each side.

```
~~Hello World~~
```

~~Hello World~~

---

## Headers

As mentioned before, the pound key ( \# ) is used in Markdown to create headers, which are the larger text used throughout the guide so far to split it into sections.  
There are six levels of headings, determined by the amount of pound signs preceding the text. One pound sign results in the largest heading, while six results in the smallest.
For example:

```
# Hello World
```

Gives:

# Hello World

While inputting

```
###### Hello World
```

Gives:

###### Hello World

All of the heading sizes are as follows:

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

Be sure to have an empty line before and after the line with your header, and to have a space between the \# and the header text.

---

## Line Spacing and Breaks

When typing lines in markdown, pressing the enter key a single time is not enough to create a new line on its own, even if it does so within the code editor.  
In order to have single line spacing, you have to end each line with two spaces before pressing enter.  
Doing so gives line spacing like in this paragraph, where each line is close together.

Alternatively, pressing enter twice gives larger line spacing, such as between the previous line and this line.

Additionally, you can enter line breaks at any point by using the break tag ( \<br> ). For example, typing this:

```
This is one continuous sentence <br> typed on only one line.
```

Will result in the following:

This is one continuous sentence <br> typed on only one line.

Additionally, a horizontal rule can be placed in with three dashes ( \- ) on a single line, like so:

```
---
```

---

## Lists, Quotes, and Code Blocks

Both ordered and unordered lists are possible with Markdown. Creating an unordered list is as simple as starting each line with a dash followed by a space, and creating an ordered list uses a number and a period followed by a space. For example:

```
- Element 1
- Element 2
- Element 3

1. Element 1
2. Element 2
3. Element 3
```

Creates:

- Element 1
- Element 2
- Element 3

1. Element 1
2. Element 2
3. Element 3

You can also indent list elements with four spaces in order to create nested lists, like so:

```
1. Element 1
2. Element 2
    a. Element 2a  
    b. Element 2b
3. Element 3
```

Creates:

1. Element 1
2. Element 2  
  a. Element 2a  
  b. Element 2b
3. Element 3

Blockquotes are done by beginning each line with a right bracket ( \> ), and can be extended by continuing to place right brackets on each line, including empty lines.

```
> This is the first line of the block quote
>
> This is the third line of the block quote
```

Creates:

> This is the first line of the block quote
>
> This is the third line of the block quote

Code blocks are what have been used to show off formatting within the grey blocks. Code blocks are created by having a line of three backtick characters ( \` ) preceding and following the lines you want within the code block. For example:

````
```
# Hello World
```
````

Text within a code block does not use any Markdown formatting, so you don't need to escape any characters - it allows you to easily show the code that is used to create things in markdown without needing to escape any of it.  
The only exception to this is trying to display triple backticks within a code block itself. To do so, make the code block out of four backticks on the preceding and following lines of the code block, rather than three. That's how I showed triple backticks in the code block above.

---

## Links

A basic link in markdown can be done by enclosing the url in angled brackets ( \< \> ).

```
<https://www.wikipedia.org/>
```

<https://www.wikipedia.org/>

Beyond this, you can control the text of a link by placing the link text in brackets ( \[ \] ), followed immediately by the url in parentheses ( ( ) ).

```
[This is a link to Wikipedia](https://www.wikipedia.org/)
```

[This is a link to Wikipedia](https://www.wikipedia.org/)

You can also add text that appears when hovering over the link by putting it inside of the parentheses, enclosed by quotation marks.

```
[This is a link to Wikipedia](https://www.wikipedia.org/ "The Free Encyclopedia")
```

[This is a link to Wikipedia](https://www.wikipedia.org/ "The Free Encyclopedia")

You can also link to headers within a document, rather than linking to a url; you can see this in action in the table of contents at the top of this document.  
To do so, format it like a normal link, but in the place of the url, put in a pound key immediately followed by the name of the text of the header you're linking to within your document.

```
[Links](#links)
```

[Basic Formatting](#basic-formatting)

The text within the parentheses must be all lowercase even if the header you're linking to has capital letters, and replace all spaces with dashes. Regardless of the header size you're linking to, only use one pound sign in the link.

---

## Tables

Tables can be created through the use of formatting with the pipe character ( \| ), using dashes ( \- ) to create headers, and using colons ( : ) to determine alignment.  

```
|  First Column   |  Second Column  |  Third Column   |
|:----------------|:---------------:|----------------:|
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |
```

| First Column | Second Column | Third Column |
|:----------------|:---------------:|----------------:|
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |

The row above the dashes becomes the header of the table.  
When formatting the row of dashes, you can determine if the column is left, center, or right aligned based on the placement of the colons.  
Having only a colon on the left of the dashes results in a left aligned column, like the First Column.  
Having a colon on either side of the dashes results in a center aligned column, like the Second Column.  
Having only a colon on the right of the dashes results in a right aligned column, like the Third Column.  





