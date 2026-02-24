<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> Feb 2026 </i></div>

 ------------

--- Feb 9th ---  
2026-02-09

Last couple of weeks ended up being especially busy, and I only managed to get a day to work on my own personal project.  

However, this week has a lot more scope for progression! So today, I started with continuing the Relic colab project! I spent most of the day working on the MVP wireframe and design in figma.  

I deliberately wanted to be careful and ensure spacing is appropriate thanks to the grid layout, that reusable components are created and stored into their own page, along with design tokens, templates, sizing & typography details.  

I'm pleased to say I managed to finish the MVP figma design for the suggested page (minus an element that's very much out of scope for now), including renaming all layers/items so it's easy to follow (I've learnt from looking at certain community figmas that consistently renamed items are so much easier to follow and understand for implementation).  I even managed to create a progress node bar component in figma, which I previously only really knew how to do in CSS.  

------------

--- Feb 10th ---  
2026-02-10

Yesterday took a surprising amount of energy, so I was glad today was more of a joint review on the Relic project, making follow-up changes to my work before allowing the current planning and design tasks to be completed. We're almost ready to start coding! 

So I spent the remainder of the afternoon returning to the Front-End Engineer career path in codecademy - 30% complete. Today was mostly recapping responsive website design & animations in CSS. 

------------

--- Feb 13th ---  
2026-02-13

For the rest of the week I've split my focus a little. I've sorted out branch rules and deployed the initial app for the Relic colab, as well as having a PR to review for the first time.  

Otherwise I've been focused on my new personal project; and I've just got a Typography system implemented and design token variables in place. I'm almost ready to deploy and work on the Layout component.  

------------

--- Feb 20th ---  
2026-02-20

This week has been very productive! 

Started with working on the Relic colab, which involved creating the Typography system and creating the design token variables (and yes, it was quicker to implement as I'd implemented this in my personal project last week!).  
With the system in place and all relevant assets loaded in, we deployed the application. Next, to actually make it worth visiting!  

I then moved back to my own project. I used a branch to tidy up some redundant styling code I'd missed, and corrected some issues I had with styling assignments (I can't believe I only just discovered that you can't use kebab-case naming conventions in Modular CSS and expect camelCase in React to function! (It either needs to be a string inside an array, or simply, make the class names in CSS camelCase).  
I then moved onto utilising react-router-dom for the first time, to make a site that is easily scalable (I'm starting with just the landing page, but this will make it easier should I create further pages).  

So today, I'm continuing to build the skeleton & styling of the Layout properly using grid; a nice task for the end of the week.  

------------

--- Feb 24th ---  
2026-02-24

Maybe a bit premature to make an entry so early in the week. However I wanted to note that I've been spending today really trying to get to grips with grid, and understand how to implement it for the site I am building.  

I initially overfocused on wanting the grid to show through every area from header to footer, much like the grid layout shown in figma. But I realise now that was a misstep.  

Using grid as a class to pass through to different sections and sub section containers made more sense.  That way I could avoid assigning those constraints to full-bleed containers but also place them inside a child container of the layout components (header & footer), leaving the parents to extend to the full width of the screen.  I also addressed an interesting edge case where I needed a container that outstretched the grid, but still took up less than a typical desktop viewport width, and realised that creating a bespoke container was the correct call for that.  

All in all, I think the landing page I had picked to translate, was not as straight forward as I thought it would be. But I've learnt a lot and I'm looking forward to seeing what else I discover whilst creating this project.

------------

<div align = "center"><a href="2026-01.md">Jan 2026</a></div>
