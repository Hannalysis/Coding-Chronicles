<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> April 2026 </i></div>

 ------------

--- Apr 3rd ---  
2026-04-03  <!-- tags:[React, TS, CSS, JS] -->

It's been a very productive week! 

As of yesterday, I managed to complete my task of making my latest personal project (the furniture site) fully responsive for all desktop sizes (mobile to follow). Meaning, I was in a good place to make that project public, and add it to my site.  

Additionally, I made some minor visual adjustments to my site; slightly lighter shade of colouring on all card types for readability, and an improved transition when the user first loads into the site.

And just before I sign off for a much needed Easter break, this morning I updated my CV project, and made adjustments to my pdf generator script.

------------

--- Apr 17th ---  
2026-04-17  <!-- tags:[React, TS, CSS, HTML] -->

After a great easter break, I'm ready and raring to get back to it this week!

I made great strides with the relic colab. It was also the first time I'd utilised a mapping system to assign styling classes to a version string:

    const versionClassMap: Record<Version, keyof typeof styles> = {
    "2.x" : "v2",
    "3.x" : "v3",
    "4.x" : "v4"
    };

This aided me in the creation of a particular dynamic component where I could add the appropriate version label to each, and still keep styling within the respective CSS module. 

I also continued with my furniture web project, and began the mobile responsive work for all common breakpoints. This was when I discovered the 'order' property, was really useful for reorganising my header on the smallest device screens so links were under header actions and the brand logo.

------------

--- Apr 24th ---  
2026-04-24  <!-- tags:[React, TS, CSS, HTML, Figma] -->

After updating the Relic colab project with a new frame in Figma to handover to my peer on Tuesday, I was free to continue my focus on my solo project for the remainder of the week. 
  
This was focused on making two sections mobile responsive ('Banner' & 'Browse The Range'), and making thoughtful layout decisions and in some cases, removing more irrelevant visuals/content to ensure the content fits on the smallest devices (320px), whilst keeping the design feel as close to the intent of the full desktop view as possible.

<div align = "center"><a href="./2026/2026-03.md">Mar 2026</a></div>