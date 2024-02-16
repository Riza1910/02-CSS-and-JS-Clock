## CSS and JS clock

This is the second project of the Javascript30 challenge.

 This project demonstrates the integration of HTML, CSS, and JavaScript to create an animated clock interface. The CSS provides the visual styling, while the JavaScript dynamically updates the clock hands to reflect the current time.

# Concepts utilised in building this project

1) CSS Transform Property:

The transform property in CSS is used to modify the appearance and layout of elements.
In the .hand class, transform: rotate(90deg); is applied to initially rotate the clock hands 90 degrees. This sets their starting position to point upwards.
When combined with JavaScript, the transform property dynamically rotates the clock hands to indicate the current time.

2) CSS Transition Property:

In the .hand class, transition: all 0.05s; is used to apply a smooth transition effect to all CSS properties when they change. This ensures that the rotation of the clock hands appears fluid and gradual.
The transition-timing-function property specifies the speed curve of the transition. In this case, cubic-bezier(0.1,2.7.0.58,1); is used to customize the timing function, creating a more natural and pleasing animation.

3) JavaScript Date Object:

The Date object in JavaScript represents a date and time.
new Date() creates a new instance of the Date object, which represents the current date and time.
Methods such as getSeconds(), getMinutes(), and getHours() are used to retrieve the seconds, minutes, and hours components of the current time, respectively.
The Date object is a fundamental tool for working with dates and times in JavaScript, allowing you to perform various operations and calculations.

4) JavaScript setInterval() Method:

The setInterval() method in JavaScript is used to repeatedly execute a function at specified intervals.
In this code, setInterval(setDate, 1000); is used to call the setDate() function every 1000 milliseconds (1 second).
It ensures that the clock hands are updated continuously to reflect the current time, creating the effect of a running clock.
setInterval() is commonly used for tasks that require periodic execution, such as updating animations, fetching data from servers, or polling for changes in the application state.