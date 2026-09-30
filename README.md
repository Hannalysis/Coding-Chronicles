<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> September 2026 </i></div>

 ------------

--- Sept 30th ---  
2026-09-30 <!-- tags:[React, CSS, Motion] -->

The busy-ness at work reached a peak this month, and has given me a chance to wind down a little as we head towards the end of the month.

Today, I thought it was a good time to make a much needed content update to my About Me section within my site.
Additionally, I saw a couple of areas where I could make small adjustments within that selfsame component for styling improvements.

Mainly, the ability for my tech stack containers to animate as they come into view (previously they'd all animate whether or not you could see them when the sidebar opens).
So, I needed to add the following properties:

```tsx
whileInView={{ opacity: 1, x: 0, y: 0 }}
viewport={{ once: true, amount: 0.2 }}
```
...and removed the redundant `animate` property entirely from this area as it's more suited to already visible elements on load, and conflicts with `whileInView`.

`whileInView` required the x and y co-ordinates specified, simply so the icons could utilise the visual zoom in from the left using the `initial` property. 
`viewport` was the property I needed to allow to animate when on display - the amount allows a percentage of that section in view before triggering.

Outside of that, I removed a bottom margin that was giving unnecessary spacing between the h3 headers within the sidebar.

------------

<div align = "center"><a href="./2026/2026-08.md">Aug 2026</a></div>
