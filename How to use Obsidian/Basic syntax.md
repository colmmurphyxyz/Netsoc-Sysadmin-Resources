---
tags:
  - howto
---

Obsidian stores notes in markdown and supports a few additional features such as links between pages, HTML and CSS support

# Headings
type 1 hashtag to create a \<h1>  element, 2 hashtags for a \<h2> and so on...
# Bold/Italic text
- surround text in double asterisks for bold
- \*\*This text is bold\*\* -> **This text is Bold**
- use single asterisks for italic, and triple asterisks for bold and italic
- __Use double underscores for underlined text__
- ~~strikethroughs are created with double tildes~~ \~\~
# Lists
- begin a line with a hyphen followed by a space to create an unordered, bullet-point list
- begin a line with a number followed by a full stop and a space to create a numbered/ordered list. Obsidian will automagically increment the number when creating new list elements
1. first element
2. second element
3. etc...
# Code
surround code with single backticks to render it in a monospace font
`System.out.println("Hello World");`
You can render blocks of code by surrounding it with triple backticks
```
def fizzbuzz(n):
	if n % 15 == 0:
		return "FizzBuzz"
	if n % 5 == 0:
		return "Buzz"
	if n % 3 == 0:
		return "Fizz"
	return ""
```
By putting a language name immediately after the first set of backticks, Obsidian will render your code with syntax highlighting
```java
public class Main {
	public static void main(String[] args) {
		System.out.println("Hello World");
	}
}
```
# Checkboxes
Obsidian supports checkboxes with a similar syntax to lists
begin a line with "- [ ]" to create a task list
- [ ] example 1
- [x] example 2
# Links
- hyperlinks are rendered with \[text here\]\(https://example.com\)
- [like this](https://www.robinsweb.com/duckpin/duck-comments.html)
- \[\[Page Name\]\] links to another page in your vault
- [[Interview Script]] <- like so
# Tables
https://www.markdownguide.org/extended-syntax/#tables
tables are kinda annoying to do, but I'm sure there exists a plugin out there to help with that
