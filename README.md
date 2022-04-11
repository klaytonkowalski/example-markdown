# Markdown

Example of Markdown language features. This document is meant as both a full Markdown tutorial and quick reference.

To learn more, visit [The Markdown Guide](https://www.markdownguide.org/) website.

Please click the "Star" button on GitHub if you find this asset to be useful!

---

## Headers

### Notes

The first method of creating a header is somewhat limited because it only supports first- and second-level headers:

```
This is a first-level header
============================

This is a second-level header
-----------------------------
```

Repeating the equals character at least twice underneath some text converts it to a first-level header.  
Repeating the hypen character at least twice underneath some text converts it to a second-level header.

The second method of creating a header is more popular because it supports first- through sixth-level headers:

```
# This is a first-level header.
## This is a second-level header.
### This is a third-level header.
#### This is a fourth-level header.
##### This is a fifth-level header.
###### This is a sixth-level header.
```

### Example

# This is a first-level header
## This is a second-level header
### This is a third-level header
#### This is a fourth-level header
##### This is a fifth-level header
###### This is a sixth-level header

---

## Spacing

### Notes

Line breaks require more than just pressing the enter key. To separate two sentences onto separate lines, add two spaces after it:

```
This is the first sentence. This is the second sentence.

This is the first sentence.  <-- Two spaces...
This is the second sentence.
```

Paragraphs do not require spaces. Instead, simply press enter twice:

```
This is the first paragraph.

This is the second paragraph.
```

### Example

This is the first sentence.  
This is the second sentence.

This is a new paragraph.

---

## Emphasis

### Notes

There are two methods for italicizing or bolding text:

```
*This is italic text.*
_This is italic text._

**This is bold text.**
__This is bold text.__
```

Bold markup is simply double italic markup.

### Example

*This is italic text.*

**This is bold text.**

---

## Links

### Notes

Links can either be pasted directly or substituted with helpful text:

```
Click here to visit my favorite search engine: https://www.google.com/

Click [here](https://www.google.com/) to visit my favorite search engine.
```

Square brackets surround the helpful text, while the parentheses surround the link itself.

Reference links are also supported. These allow a link to be assigned an identifier, which is then defined somewhere else in the document:

```
Click [here][identifier_1] to visit my favorite search engine.  
Or try [this][identifier_2] one!

[identifier_1]: https://www.google.com/
[identifier_2]: https://duckduckgo.com/
```

Note that both the helpful text and the identifier are surrounded with square brackets. Parentheses are not present.

### Example

Click here to visit my favorite search engine: https://www.google.com/

Click [here](https://www.google.com/) to visit my favorite search engine.

---

## Images

### Notes

Similar to links, images are embedded using square brackets and parentheses, but also include a prepended exclamation point:

```
![Picture of bananas](https://cdn1.sph.harvard.edu/wp-content/uploads/sites/30/2018/08/bananas-1354785_1920-1024x683.jpg)

![Picture of bananas][identifier]

[identifier]: https://cdn1.sph.harvard.edu/wp-content/uploads/sites/30/2018/08/bananas-1354785_1920-1024x683.jpg
```

Note that the image's [alt text](https://www.w3schools.com/tags/att_img_alt.asp) is placed inside the square brackets.

### Example

![Picture of bananas](https://cdn1.sph.harvard.edu/wp-content/uploads/sites/30/2018/08/bananas-1354785_1920-1024x683.jpg)

---

## Lists

### Notes

Lists can be either ordered or unordered. Ordered lists use numbers, while unordered lists use the asterisk, hyphen, or plus characters:

```
1. Alpha
2. Beta
3. Gamma

* Alpha
* Beta
* Gamma

- Alpha
- Beta
- Gamma

+ Alpha
+ Beta
+ Gamma
```

Line breaks and paragraphs can be inserted within list items:

```
1. Alpha  
   The first character in the Greek alphabet.
2. Beta
   The second character in the Greek alphabet.
   Also refers to an in-development version of software.
3. Gamma
   The third character in the Greek alphabet.
   
   Gamma is often substituted by "Charlie" in situations where verbal clarity is especially important.

4. More characters...
```

Finally, lists can be nested. Nested lists do not need to match their parent's ordered or unordered property:

```
1. Alpha
2. Beta
   1. B
   2. e
   3. t
   4. a
      * The first character in the English alphabet.
      * The first letter in the word "apple".
3. Gamma
   * G
   * a
   * m
   * m
   * a
```

### Example

1. Alpha
2. Beta
   1. B
   2. e
   3. t
   4. a
      * The first character in the English alphabet.  
        ...And many other alphabets!
      * The first letter in the word "apple".
3. Gamma
   * G
   * a
   * m
   * m
   * a

---

## Blockquotes

### Notes

It is important to indicate when the words you use are not your own! Blockquotes use the right angle bracket:

```
> Battle not with monsters, lest ye become a monster, and if you gaze into the abyss, the abyss gazes also into you.
```

Blockquotes can be nested by adding extra right angle brackets:

```
> Battle not with monsters, lest ye become a monster, and if you gaze into the abyss, the abyss gazes also into you.
> > Friedrich Nietzsche
```

### Example

> Battle not with monsters, lest ye become a monster, and if you gaze into the abyss, the abyss gazes also into you.
> > Friedrich Nietzsche

---

## Code

### Notes

Program code can be inlined with one or more backticks:

`````
Use the C++ `<iostream>` header for input and output.

It should look something like this:

```
#include <iostream>
std::cout << "Hello, world!\n"
```
`````

Note that using three or more backticks will escape all other Markdown characters within the code.

Unlike inline code, preformatted code blocks do not wrap and always display their contents exactly as typed. Use four spaces or one tab before each line:

```
    #include <iostream>
    int main(int argc, char *argv[])
    {
        std::cout << "Hello, world!\n";
        return 0;
    }
^^^^
Four spaces...
```

### Example

Use the C++ `<iostream>` header for input and output:

    #include <iostream>
    int main(int argc, char *argv[])
    {
        std::cout << "Hello, world!\n";
        return 0;
    }

---

## Horizontal Lines

### Notes

Great for readability, horizontal lines use three hyphens or asterisks:

```
Section 1
---
Section 2
***
Section 3
```

### Example

---
