# <img src="https://avatars.githubusercontent.com/u/11639138?v=3&s=30" style="vertical-align: middle"> scroll-link <span align="right"></span>
Polymer component for native smooth scroll behavior. 

Based on [Scroll Behavior polyfill](https://github.com/iamdustan/smoothscroll)

## Install
Install with bower: 
```
bower install scroll-link
```
## Usage

### Scroll to page element
```html
<!doctype html>
<html>
  <head>
      <title>My Polymer App</title>
    <script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="bower_components/scroll-link/scroll-link.html">
    </head>
    <body>
        <scroll-link href="#about" title="link title">About section</scroll-link>
        ...
        <section id="about">
            some content
        </section>
    </body>
</html>
```
### Scroll to position
```html
<!doctype html>
<html>
  <head>
      <title>My Polymer App</title>
    <script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="bower_components/scroll-link/scroll-link.html">
    </head>
    <body>
        <scroll-link top="200" left="50" title="link title">Scroll to position top: 200px, left: 50px</scroll-link>
    </body>
</html>
```
## Attribute properties 
 * __href="selector"__ - scroll to html selector (document.querySelector). Prefer then "top"/"left";
 * __top="Number"__ - scroll to top position
 * __left="Number"__ - scroll to top position
## Styling
Free for changes!
### CSS Custom Properties
```css
    --scroll-link-display: block; /* chage display scroll-link host component*/
```

### CSS component customization
Example:
```css
scroll-link {
    backgroud:red;
    margin: 10px;
    color: blue;
}
scroll-link > a {
    text-decoration: none;
    font: 17px/1 'Helvetica', sans-serif;
}
```

## Roadmap
* Scroll from Right/Bottom, ScrollBy
* Demo
* Add to Polymer Catalog
* Tests