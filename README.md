# Font-Awesome-For-Ionic-Tabs
Use Font Awesome icons with Ionic Framework tabs

## Installation
Make sure you have Font Awesome installed correctly and is working with your Ionic app. You'll need to make sure the fonts are located locally on in your app and that your @font-face src is correctly pointing to files.

Then include the font-awesome-ionic-tabs.css file in your app. If it's working correctly, you should be able to use the classes just like the ionicons.


```html
<ion-tab title="Photos" icon-on="ion-tab-fa-anchor" icon-off="ion-tab-fa-anchor">
  <ion-nav-view name="tab-one"></ion-nav-view>
</ion-tab>
```

## Adding Fonts
***NOTE:*** I have not added all of the Font Awesome icons to the style sheet yet. Feel free to help! 

* Find the unicode characters here: http://fortawesome.github.io/Font-Awesome/cheatsheet/
* See if they are already included in this list
* Name your style identical to the font awesome style, but prefix with "ion-tab-"
* Add in two places (CSS description at top and the specific content: with the unicode)

*Example before...*

```css
.ion-tab-fa-anchor:before   {
  display: inline-block;
  font-family: "FontAwesome";
  font-size: 72%;
  speak: none;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  text-rendering: auto;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; }

.ion-tab-fa-anchor:before {
  content: "\f13d"; }
```

*Example after...*

```css
.ion-tab-fa-anchor:before, .ion-tab-fa-apple:before   {
  display: inline-block;
  font-family: "FontAwesome";
  font-size: 72%;
  speak: none;
  font-style: normal;
  font-weight: normal;
  font-variant: normal;
  text-transform: none;
  text-rendering: auto;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; }

.ion-tab-fa-anchor:before {
  content: "\f13d"; }
  
 .ion-tab-fa-apple:before {
  content: "\f179"; }
```

*Now you can use your new class...*

```html
<ion-tab title="Photos" icon-on="ion-tab-fa-apple" icon-off="ion-tab-fa-apple">
  <ion-nav-view name="tab-one"></ion-nav-view>
</ion-tab>
```


