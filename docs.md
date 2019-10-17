# matty engine
```js
mattyEngine.start(q) 
// Starts a new instance of Matty Engine. Parameter q is a querySelector 
// of a document on the page, of which the game will be appended to.

mattyEngine.setBackground(i) 
// Sets the background of the Matty Engine document. 
// Parameter i is an image to use. Should be a directory e.x. /path/to/img.png

mattyEngine.newDialog(t)
// Pushes text to the back of the mattyEngine text queue.
// Parameter t is the text to push.

mattyEngine.clearQueue()
// Clears the text queue and cancels the current dialog. 

mattyEngine.dialogAdvance()
// Advance the text queue, similar to pressing ENTER.

const CHARACTER = mattyEngine.newCharacter(s, p, h, o)
// Creates a new Matty Engine character. Parameters:
// S: Image used for the character. Should be a directory e.x. /path/to/img.png
// P: The place of the Matty Engine character. From 1-100, will be the % to the right.
// H: The height of the character. Should be in pixels.
// O: Callback on click. Should be a function.

CHARACTER.src(s)
// Change the image source. Parameter s should be a directory e.x. /path/to/img.png

CHARACTER.delete()
// Delete the character.

CHARACTER.move(l)
// Move the character. Parameter l should be 0-100, % to the right.

CHARACTER.click(c)
// Change the function that fires when the character is clicked.
// Parameter c is said function.
```
