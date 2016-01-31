# The layout of the web
There has been a lot of discussion about the fact that HTML wasn't designed for web apps. HTML provides two general purpose primitive tags `div` and `span` and then a *whole lot of CSS* to style and layout this and other tags to your hearts content. But lets take a step back and imagine how a framework *desgined for application layouts* would look like.

# Reusing ideas of the past
XAML was a technology designed for layout. However there is nothing about HTML that prevents us from using the lessons there and using them to create a reliable layout system for the web.

# Basics
There are very few simple things about the default layout of an HTML page that need to be setup in order to prepare it for the application era:

* Full Sized Body
* Box Layout

## Full Sized Body
You really want the root of your page to be something that takes up all the available space on screen and provides it as a drawing canvas for children.

```css
html, body {
    height: 100%;
    width: 100%;
    padding: 0px;
    margin: 0px;
}
```

# Rethinking the primitives
If one was creating something for HTML today for application layout you would need a
