<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> July 2025 </i></div>

 ------------

--- July 10th ---  
2025-07-10

I have been quiet on my personal coding learning journey for the last few weeks, as I wanted to focus my efforts at work whilst there was a major event we needed the project to be ready for, and I was already learning so much about being a Back-End developer from the experience. 

So after completing my contract (and giving myself a much needed break), I am ready to get back to it. I have made so many plans and items that require actioning.  

My priority today returned me to my colab project with my mentor - whom I managed to have a catch-up with earlier this week. I finally got to discuss my UI/UX wireframes I'd created in Figma for our 1st round/game mode of choice and decide our overall app approach.
So today I created a Github project and added all tasks we have agreed to action for our MVP/MS1. 
I've already noticed the limitations of Github projects compared to my previous experience with Jira, and had to create some workarounds (mostly by making custom fields that act as tags/labels).  

I then actioned my first task, by researching into appropriate folder hierarchy structures for our repo, and is now review ready - so I can then implement this as the next step.  

------------

--- July 11th ---  
2025-07-11 

Due to early confirmation for the folder structure suggestion, I spent today creating the scaffolding for the colab project. This also included converting the App.css file to be modular, which then caused me to need to update the App.tsx file so the styling would persist.  
It also made me realise that the React Vite boilerplate utilises global CSS inside the App.css file, so I moved the culprits to the index.css file and made an additional styling property to justify the body's content to be centred once more.  

With a PR awaiting review to hopefully merge and close the relevant Github issue, I decided to leave it there for today as it's very hot and my PC is not helping! 

------------

--- July 12th ---  
2025-07-12  

Today I decided was a good time to begin refactoring my CV. In particular, I want it to closer match my portfolio branding.  

As I created my portfolio in React with TypeScript, I thought it would be best to refactor my CV in the same tech stack, and move away from plain HTML & CSS.  
So today I initiated the project, and started by testing portfolio components to see if they would render with the puppeteer pdf capture.  To my guess, it had issues with capturing framer motion animated components when they had fully rendered.  
Puppeteer did not seem to like waiting for a timeout with React, so I tried the useReducedMotion function from motion - which improved the capture visuals slightly. But ultimately I decided I had to wholesale remove framer-motion from any element that did not render in time for the capture.  

Fortunately that was the solution, so next time I'm focusing on this project, I can get down with designing, wireframing if needed and then start a basic implementation.  

------------

<div align = "center"><i><a href="2025-05.md">May 2025</a></i></div>
