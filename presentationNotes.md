# Title slide

- Show interview.ueno.co (made with greensock)
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
- So code along, click codepen link and let's try it out
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
