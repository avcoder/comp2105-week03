# Title slide

- Play https://flukeout.github.io/
- CSS transforms - this is the basics of animation
- transforms, transitions, translate - can be confusing

# To Do

- open up my slides if you haven't done so
- this will be very interactive class

# Val Head quote

- my example: transforms is like pose to pose vs transitions is like straight ahead

# CSS Transforms

- you know when you adjust padding -> affects other elements on page
- transforms do not do that

# Syntax

- syntax of transforms looks like this: transform: function(parameters)
- see link MDN docs to see all the different variations
- the 4 major ones we'll be using mostly are: translate, scale, skew, rotate = 2D
- vs. "3d" "Z"
- ignore matrix

# 2D

- when you're doing 2D transforms, think of these 4
- icons remind you what they do
- scale: like squash & stretch
- skew: like follow thru/overlapping
- translate: move an object sideways/up/down, like float
- rotate: clockwise / counter
- so those are the 4 main ones for transform
- keep in mind, when you're animating, it's not just limited to these 4 but also other animatable properties as well (see link) such as background-color etc.
- today we'll just focus on these 4
- Review: what are the 2 most performant properties? transform and opacity

# scale

- in 2D, you'll be using 1 of these 4 possibilities
- So code along, click codepen link, FORK it, and let's try it out
- 1st example: you tell me does this scale x? y? both?
- 2nd example: if you want to specify x
- What do you anticipate this would look like? This should stretch but height should remain same.
- 3rd example: you can specify y
- What do you anticipate? height to change only
- 4th example:
- try to imagine what this might look like before I hover - important to try to have mental models
- always include the word transform in your CSS otherwise it won't work
- now you might be asking yourself, but it's not smoothly animating?
- add transitions to buttons ; but we'll get into that next week

# skew

- read it
- So code along, click codepen link and let's try it out
- Instead of hovering to trigger, what CSS would you write to make it trigger on click event?
- one mental model that helps me is that if it's skewX, since X = horizontal, then horizontal lines will stay the same
- if you took a corner of the shape and pulled it, with point of origin at center, it skews

# translate

- read it
- I got this example from last year's class (show treefrog.ca)
- try to emulate this using css transform
- it won't get us the whole way, there's a few details still missing
- for translateY what kind of value makes it go up? positive or negative?
- for translateX what kind of value makes it go right/left?

# rotate

- Challenge: rotate element upon click but use JS click events to toggle a class called 'rotate'
- once finished: Notice point of origin is in the middle
- because if the point of origin was shifted to the bottom left corner, and then rotate it, it won't rotate in the middle anymore. We'll get into that in a moment

# transform-origin

- see link
- notice the values can be px, or keywords, or percentages
- let's try changing the point of origin / transform-origin for previous example

# transform-origin codepen

- go into codepen
- now add in a transform-origin to the bottom left corner
- try to predict how this will move before I click it
- it helps to put a border and a transition to see what's really happening
- encourage you to experiment with different values, like top right etc.

# multiple values

- you can also have multiple values on the same line
- 1st example: here the transform has 2
- 2nd example: has 3
- try to imagine what will happen before I click it

# Quiz 3

- you'll be able to answer 5 questions for now, you can do the other 5 later
- by forcing you to guess something you don't know that's a good form of deep learning

# 3d val quote

# 3d

- so just like previously for 2d you had to know the 4 transforms (scale translate skew rotate)
- in 3d you have to know (read it)

# codepen 3d

- hold paper, y axis is vertical
- so you must add perspective first

# codepen perspective 100 to 100 in 3s

- so here we have 1000px perspective, then 3 seconds later it moves to 100px perspective
- Q: which one looks closer to you? 1000px vs 100px?
- the closer/lower the value, the more closer it seems, the more distorted the effect

# codepen perspective-origin

- just like in 2d you had transform-origin, in 3d you have perspective-origin
