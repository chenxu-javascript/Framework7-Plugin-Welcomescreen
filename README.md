# Framework7 Plugin Welcomescreen

## Just a quick plugin for Framework 7

This will display a fullscreen swipeable modal window to guide the user through a welcome screen.

## Live demo

http://www.timo-ernst.net/misc/f7-plugin-welcomescreen

## Dependencies

- Swiper (http://www.idangero.us/swiper/#.VR_1mlz5JoI)

## Setup

1) Make sure you have Swiper installed. See /example folder on how to do it and read the docs on http://www.idangero.us/swiper/#.VR_1mlz5JoI

2) Copy welcomescreen.css and welcomescreen.js to your project and reference them:

```html
<link rel="stylesheet" href="welcomescreen.css">
<script src="welcomescreen.js"></script>
```

3) Import welcomescreen lib in javascript

```javascript
var app = new Framework7();
var welcomescreen = myapp.welcomescreen(options);
```

4) Create some slides. You can use any html as parameter "contenthtml".

```javascript
var welcomescreen_slides = [
  {
    id: 0,
    contenthtml: '<div><br><br><br>Welcome user, this is slide 1<br>Swipe right to see next tutorial page</div>'
  },
  {
    id: 1,
    contenthtml: '<div><br><br><br>This is slide 2</div>'
  },
  {
    id: 2,
    contenthtml: '<div><br><br><br>This is slide 3</div>'
  },
  {
    id: 3,
    contenthtml: '<div><br><br><br>This is slide 4</div>'
  }
];
```

5) Initialize welcome screen

```javascript
welcomescreen.addSlides(welcomescreen_slides);
```

That's it :-)
Enjoy

Made with <3 by www.timo-ernst.net
