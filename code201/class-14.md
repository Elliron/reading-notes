# Transforms
- **transform** 2 different settings
  - two-dimensional
      - work on x and y axis
      - horizontal axis
      - vertical axis
    - rotate
      - o to 360 degrees
    - scale
      - changed appeared size of element
      - default value of 1
      - scaleX and scaleY
    - translate
      - positioning, push and pull element in different directions without interupting flow
      - translateX
      - translateY
    - skew
      - distorts elements on horizontal, vertical or both axis's
      - skewX
      - skewY
    - combine transforms

    ```
    .box-1 {
      transform: rotate(25deg scale(.75);)
    }

    .box-2 {
      transform: skew(10deg, 20deg) translateX(20px);
    }
    ```

    - origin
      - one or two values
      - one value = horizontal and vertical axis
      - two value = first for horizontal, second for vertical

  - three-dimensional
      - x, y and z axis
      - length
      - width
      - depth
    - perspective
      - perspective which to transform
      - thought of as vanishing point
      - use perspective value within transform property on indvidual elements, great for single
      - use perspective value on parent element residing over child elements being transformed, great for group
    - perspective depth value
      - can be set as none or a length measurement
      - none turns off any perspective
      - higher value, further away perspective appears
    - perspective-origin 
      - same values for transform-origin property may be used
      - origin of perspective identifies coordinates of vanishing point
    - three-dimensional transforms
      - 3rd axis
      - 3D rotate
        - rotateX
        - rotateY
        - rotateZ
      - 3D Scale
        - scaleZ
      - 3D translate
        - translateZ value, translates on z axis
          - negative value will push element further away on z, positive pull closer
      - 3D Skew
        - cannot be transformed on three-dimensional scale
      - Transform Style
        - three-dimensional transforms applies on element, nested within parent element which is also being transformed
        - transform-style property
          - preserve-3d
          - flat
      - Backface Visibilty
        - faced away from screen
        - shown from back
        - set to *hidden* if you don't want to see
        - default value is visible


# Transitions and Animations
- alter appearance and behavior of an element when state change occurs

### transitions
  - :hover
  - :focus
  - :active
  - :target
- transition-property
  - what properties with be altered in conjunction with other transitional properties
  - only properties with identifiable halfway point may be transitioned
- transition-duration
  - set using general timing values; seconds, milliseconds etc
- transition-timing-function
  - set speed of transition
  - linear, ease-in, ease-in-out
- transition-delay
  - sets time value, seconds or ms, determines how long transition stalls before executing

### Animations
- @keyframes

```
@keyframes slide {
0% {
  left: 0;
  top: 0;
}
50% {
  left: 244px;
  top: 100px;
}
100% {
  left: 488px;
  top: 0;
 }
}
```

```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-fill-mode: forwards;
}
.stage:active .ball {
  animation-plate-state:paused;
}
```

#### Shorthand

```
.stage:hover .ball {
  animation: slide 2s ease-in-out .5s infinite alternate;
}
.stage:active .ball {
  animation-play-state: paused;
}
```

#### CSS3 Transitions
- Fade in
- Change color
- Grow and Shrink
- Rotate elements
- Square to circle
- 3D shadow
- Swing
- Inset border

# Google
- data saturated age
  - enables us to examine our work habits and office quirks
- employee performance optimization
  - isn't enough
- work is more and more team based
- groups innovate, find mistakes and find better solutions faster
- groups report better results and higher job satisfaction
- Googles People Operations
  - study every aspect of peoples lives, what makes good employees and managers
- Project Aristotle
  - study hundreds of Google's teams
  - couldn't find an answer, the "who" didn't matter
  - group norms
    - "unwritten rule"
    - "team's culture"
  - successful groups
    - "equality in distribution of conversational turn-talking" everyone speaks roughly the same amount of time
    - high "average social sensitivity" skilled at intuiting how others felt based on tone of voice 
    - **psychological safety**

[Home](../README.md)