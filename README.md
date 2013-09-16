Tetris
======

Tetris in Smalltalk.

![alt tag](https://raw.github.com/paoloboschini/tetris/master/screen1.png)
![alt tag](https://raw.github.com/paoloboschini/tetris/master/screen2.png)

Installation
======

Go to http://www.pharo-project.org/home and download the Pharo 2.0 one-click distribution.
Open it, click in the world and go to tools menu -> file browser.
Locate the file Tetris.st you cloned from this repo, select it and choose Filein.
Now the Tetris category is imported into your image.

Run
======

Click in the world, open a new Workspace, and type

**TaskbarMorph showTaskbar: false.**

**TetrisGame start.**

and Do It (cmd+d or from the menu)!

TODO
======

Refactor!

MISC
======

My favourite line, reflection! :)

```smalltalk
createSprite
	^ (Sprite subclasses at: (Random new nextInt: Sprite subclasses size)) new position: self position + (150 @ -50)
```