
Markdown quick reference
See the Markdown page for instructions on enabling Markdown for posts, pages and comments on your blog, and for more detailed information about using Markdown.

Markdown	Processed
Emphasis	
*Emphasize* _emphasize_
**Strong** __Strong__
Emphasize
Strong
Some WordPress.com themes may have different formatting for these styles

Inline Links	
A [link](http://example.com "Title").
Most browsers show the title text when hovering over a link.
Please note that WordPress shortcodes, like [video] or [audio], will take priority over Markdown links and shouldn’t be used for link text.

A link.
Referenced Links	
Some text with [a link][1] and
another [link][2].

[1]: http://example.com/ "Title"
[2]: http://example.org/ "Title"
The reference section can be anywhere in the document

Some text with a link and another link.
Inline Images	
Logo: ![Alt](/wp.png "Title")
The “Alt” text (alternative text) makes images accessible to visually impaired

Logo: Alt
Referenced Images	
Smaller logo: ![Alt][1]

[1]: /wp-smaller.png "Title"
Smaller logo: Alt text
Linked Images	
Linked logo: [![alt text](/wp-smaller.png)]
(http://wordpress.com/ "Title")
Linked logo: alt text
Footnotes	
I have more [^1] to say up here.

[^1]: To say down here.
Footnotes will be added to the bottom of the document, with a link back to the original reference

I have more 1 to say up here.
To say down here. ↩
Line breaks	We do not support Markdown’s typical double-space to generate a line break due to our built-in auto-linebreaking function. A regular line break will generate a line break on output.	 
Bullet Lists	
* Item
* Item
- Item
- Item
Item
Item
Item
Item
Numbered Lists	
1. Item
2. Item
Item
Item
Mixed Lists	
1. Item
2. Item
   * Mixed
   * Mixed  
3. Item
Item
Item
Mixed
Mixed
Item
Blockquotes	
> Quoted text.
> > Quoted quote.

> * Quoted 
> * List
Quoted text.

Quoted quote.

Quoted
List
Preformatted	
  Begin each line with 
  two spaces or more to 
  make text look
  e x a c t l y 
  like  you  type i
  t.
Begin each line with 
two spaces or more to 
make text look
e x a c t l y 
like  you  type i
t.
Code	
`This is code`
This is code
Code block	
~~~~
This is a 
piece of code 
in a block
~~~~

```
This too
```
1
2
3
This is a
piece of code
in a block
1
This too
Syntax highlighting	
```css
#button {
    border: none;
}
```
See Posting Source Code for supported languages

1
2
3
#button {
    border: none;
}
Headers	
# Header 1
## Header 2
### Header 3 
#### Header 4 ####
##### Header 5 #####
###### Header 6 ######
Closing hash marks are optional on all levels

Header 1

Header 2

Header 3

Header 4

Header 5

Header 6

Definition Lists	
WordPress
:  A semantic personal publishing platform 

Markdown
:  Text-to-HTML conversion tool
WordPress
A semantic personal publishing platform
Markdown
Text-to-HTML conversion tool
Formatting for definition lists may vary between themes

Abbreviations	
Markdown converts text to HTML.

*[HTML]: HyperText Markup Language
Definitions can be anywhere in the document

Markdown converts text to HTML.
These are some of the most useful Markdown features available on WordPress.com. See the official Markdown project and Markdown Extra for details about all available features, and variations on the features mentioned here
