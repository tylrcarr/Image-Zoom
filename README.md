# So this is a simple image zoomer I made in the process of making a website to get into a program.
## I got kinda sick of having to supply a smaller image, so I did it using canvas.
All you have to do is supply a id for that image you want to canvasify and create the zoom effect for

All you need to do is run 

```javascript
$(/* your identifier here */).zoom();
```

That's it.

Your options are as follows: 

### Zoom

DEFAULT: 5

```javascript
$(/* your identifier here */).zoom({zoom: 2});
```
Zoom is just the level of zoom on the image.

It's calculated by dividing the width by the zoom level. 

So, if my width were the size of my image, and the zoom were 2, you'd see a little less than half the image (because of the circle effect)

### Width & Height

DEFAULT: 250

```javascript
$(/* your identifier here */).zoom({width: 500, height: 400});
```

These 2 variables are pretty self explanatory. It's the width and height in PX of the zoom reticle

If the height or width is bigger than the image, it's resized to size of the image. If this is an issue to you for some reason, you can change the...

### Auto-correct Height / Width 

DEFAULT: True

```javascript
$(/* your identifier here */).zoom({width: 500, height: 400, autoCorrect: false});
```

This changes the aformentioned issue. I can't forsee a reason for it, but Facebook was written in PHP and they didn't see a reason why not to until it was far too late.

## THAT'S IT. 

If you have any improvements to the project, feel free to make that request. I wrote this in under 2 hours, so I wouldn't be suprised if it had some bugs.

## License

Includes the "Don't Be a Dick" license. Read the license if you feel the need to.
