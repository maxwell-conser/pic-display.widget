# pic-display.widget
Very tiny, very simple widget to put a picture on your desktop via Ubersicht.

The main purpose of this is to allow other Ubersicht widgets to be overlayed with the desktop as seen ![alt text]
(Example/Screenshot-Final.png). In that example the pic-display widget with [this picture](Example/Picture-To-Overlay.png) was overlayed on one of the default Yosemite desktop backgrounds with the clock widget in between.

## How to use.

The command echoes back the location of the image you want to display. Simply change the default file path to point towards your image.

It is recommended that you put your picture in the `pic-display.widget/Pics` folder, then it is stored locally and you only have to change `YOUR_IMAGE_HERE.png` to the name of your image. If for some reason you don't want to store it locally you can also use a URL in place of a path.

Any normal web image format will work -- i.e. JPEGs, PNGs, or even animated GIFs.

You can use the [z-index](http://www.w3schools.com/cssref/pr_pos_z-index.asp) to control which widget goes on top of which, for example in [the picture above](Example/Screenshot-Final.png) I added `z-index: -1` to the style of the clock widget to make sure it appears behind the picture.

If you are trying to put some widget under the desktop image like in the Yosemite example above, do yourself a favor and use a screenshot to select the [image overlay](Example/Picture-To-Overlay.png) from. By taking a screenshot you know your overlay is the exact right size and you won't have to finagle with the width.
You will usually have to mess with the placement of the image to get it to overlap properly, even if it's only by moving it down 1.5% or whatever.
