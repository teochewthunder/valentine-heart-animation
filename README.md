# Valentine Heart Animation

For this, a HTML file with a div (id *placeholder*) and script links to jQuery and the jQuery Animation API are required.

## Preparation
### HTML/CSS
*Placeholder* and divs within paceholder will not have *height* and *width* pre-defined.

### JavaScript
An object, objAnimation is created. This will store properties such as sizes, colors and content.
- *shape* is a two-dimensional array that holds defines the grid.
- *render()* is a method which draws the grid on screen.
- *generateRandomNo()* is a method that generates a number between *min* and *max*.

## Implementation
### *objAnimation.render()*
This takes the *shape* property and creates a square div for each element. These divs have *unitSize* width and height. *placeholder* will thus have (*unitsize* x *shape.length*) pixels width and height.

Each div has *content* inside it. In this case, we use the &hearts; symbol, forming many small hearts within a larger heart (the grid).

### *objAnimation.animateObject(animateId)*
Each animation (defined by *animateId*) will iterate through the *shape* object in various ways and run the *objAnimation.animateColor()* or *objAnimation.animateSize()* or both on each element, giving rise to several interesting effects!

### *objAnimation.animateColor(obj, delay, color)*
Uses the Animation API to animate *obj*'s *color* property with a duration of *delay* ms.

### *objAnimation.animateSize(obj, delay, size)*
Uses the Animation API to animate *obj*'s *size* property with a duration of *delay* ms.


