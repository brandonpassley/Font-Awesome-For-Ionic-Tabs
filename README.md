# Font-Awesome-For-Ionic-Tabs
Use Font Awesome icons with Ionic Framework tabs. Includes icons from Font Awesome 4.5.0 (thanks to [@ollycross](https://github.com/ollycross))

## Installation
Make sure you have Font Awesome installed correctly and is working with your Ionic app. You'll need to make sure the fonts are located locally on in your app and that your @font-face src is correctly pointing to files.

Then include the font-awesome-ionic-tabs.css file in your app. If it's working correctly, you should be able to use the classes just like the ionicons.


```html
<ion-tab title="Photos" icon-on="ion-tab-fa-anchor" icon-off="ion-tab-fa-anchor">
  <ion-nav-view name="tab-one"></ion-nav-view>
</ion-tab>
```

## Adding Font Awesome Icons
* Find the unicode characters here: http://fortawesome.github.io/Font-Awesome/cheatsheet/
* See if they are already included in this list
* Name your style identical to the font awesome style, but prefix with "ion-tab-"
* Add the class with the unicode content to the list

*Example...*

```css
.ion-tab-fa-anchor:before {
  content: "\f13d"; }
```

*Now you can use your new class...*

```html
<ion-tab title="Photos" icon-on="ion-tab-fa-anchor:before" icon-off="ion-tab-fa-anchor:before">
  <ion-nav-view name="tab-one"></ion-nav-view>
</ion-tab>
```


