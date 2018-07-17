
# Put one # for Header1, 
## Put two ## for Header2, 
### Put three ### for Header3, 
#### Put four #### for Header4

Put `single backticks` to shade in the text as shown.

- A single dash then space "- " before a line ends up looking like this.

<Text between angle brackets looks like this>
<summary>Text between summary tags looks like this</summary>
<p>Open a new paragraph here

```javascript
  Enclosing something in 3 backticks looks like this. RadioGroup.prototype.handleKeyDown = function(e) {
    switch(e.keyCode) {

      case VK_UP:
      case VK_LEFT: {
        
        e.preventDefault();

        if (this.focusedIdx === 0) {
          this.focusedIdx = this.buttons.length - 1;
        }
        else {
          this.focusedIdx -= 1;
        }
        
        break;

      }

      case VK_DOWN:
      case VK_RIGHT: {

        e.preventDefault();

        if (this.focusedIdx === this.buttons.length -1) {
          this.focusedIdx = 0;
        }
        else {
          this.focusedIdx += 1;
        }

        break;
      }

    }

    this.changeFocus(this.focusedIdx); // <-- Hmm, interesting...
  };
```
Close paragraph here
</p>
Close details here
</details>

- - -
Next up: [Text between square brackets](ND024_Part2_Lesson11_15.md) or return to [Text2 betw square brackets](./ND024_TableOfContents.md)
