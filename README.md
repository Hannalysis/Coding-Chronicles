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

--- July 13th ---  
2025-07-13

Today was a continuation on refactoring my CV.  To speed me up, I used v0 dev to generate a basic template with components. Utilising a tidier structure than provided, I plugged in each component and added modular CSS to each one.  

What I found useful today was how easy it is to plug and switch my portfolio template file, to the CV file and then run the build.  This project may end up having an additional use case - once I'm ready to update my Github profile repo image and Linkedin background. 

I then spent the remainder of my allocated time setting up my colour palette within the :root and applied it throughout the project. I also played around with some grid css to create a more fluent split column on the top container of sections. 

Finally, I added my branding divider just under the Hero section, checked puppeteer could capture the image, before pushing up the local changes.

------------

--- July 14th ---  
2025-07-14

Today I thought to return to my Associate Data Engineer in SQL career track in Datacamp, and continue the Intermediate SQL course.

I managed to complete the last two chapters, which focused on filtering and aggregating, sorting and grouping. This was also the first time I was introduced to the HAVING keyword, which is utilised for filtering grouped records. It was also interesting as I realised you cannot utilise aliases on this query type, and are only effective on ORDER BY
filters.  I also learnt the differences of written code of SQL and the order of execution for these additional keywords that were covered in this course. 

Overall career track completion - 33%.  

I finished up by doing a few additions and fixes to my CV refactor project - added global styling for list items, fixed the custom divider so it displays the correct length of patterned squares on the pdf, and started testing out some card styling changes.  

------------

--- July 16th ---  
2025-07-16

Due to adulting admin and appointments to make, today wasn't a great day for in-depth taskwork.  So I continued with my CV refactor, but focused on the smaller changes; the visual colouring and sizing tweaks, and the dynamic container logic.  

I added dynamic containers appropriate to the amount of certifications and adjusted so only two would align in a column, and 3 columns would fit into a single container. If there was an odd amount, one would appropriately fit into it's own container.  
I had a similar setup with less columns for Education & Journals.  

After re-shuffling the components inside the template tsx (aka the App tsx) to move what I believe is more relevant to be more front-facing on the pdf output - I focused on giving all card-based components the same styling that overall fits with my theme, without removing the readability of the content.   

I also re-sized and justified the link icons for both the Journals and Projects section. And after fending off a pesky html element that happened to be classless inside a modular CSS file, I left it there for today.  

------------

--- July 17th ---  
2025-07-17

Today I spent time back on my career track in Datacamp.  

I completed the first chapter of the Joining Data in SQL course; which was almost entirely INNER JOIN focused. This also included learning the USING command and chaining INNER JOINS queries.  

I found the idea to work on creating the INNER JOIN and FROM part of the queries first (as we needed to alias them) then moving onto the SELECT was not as fluid as I was hoping for, but I will get used to it (and ultimately, makes sense as you need to know what the aliases are before SELECTing them.)   

I finished up with some experimentation with my smaller square diamond divider component for my CV refactor. Ultimately, it looked a little busy and I settled with the addition inside the Footer only, and instead styled the line Dividers to have less opacity and better spacing.  

------------

--- July 18th ---  
2025-07-18

Today I continued working on my CV refactor project.  

I started with refactor a little more of the styling; I realised I had a couple of additional colourings that I was utilising on many components, so I added them to the :root and then distributed the variable on the appropriate module css files for more clarity, and also futureproofing any potential theme changes with ease.  

I then encountered an interesting bug with my small line SectionDivider components.  One of my section dividers was not displaying when capturing it through puppeteer, but was fine when viewing it through React.   It was not the last component and would not be the last item to load, so I did not believe it was a premature capture before fully rendering, but I checked to be sure.  No matter what delay I set, the capture was the same. I decided to start placing additional dividers, and some would display, others wouldn't. I tried copying more of my other graphically intensive dividers but they all captured with no issue.  I also created a separate component, but with the same code and styling as the section divider to no avail.

Luckily, I was able to chat to a fellow developer about my issue, and we debugged it together.  They noticed that it was mathematically every 3 of the culprit section dividers were not capturing.  Once I had also informed them about my separate component attempt that also did not render on capture, we starting looking at the styling of the section divider itself.  
They noticed I was utilising sub pixel sizes (0.75px) for those particular borders, so we changed them to a whole integer, then started the capture. That was the fix! I did not realise that puppeteer utilises headless Chromium, which does not behave as a fully rendered browser would. It's possible it can get rounded, and therefore not render/renders invisible. 

With that sorted I commited and pushed my changes, and then stepped away from another heat-intensive day.  

------------

--- July 19th ---  
2025-07-19

Today I was determined to get my CV refactor project in a state where I could input content from a json file, and pass it through as props to the necessary components of the React App.   
  
Refactoring the component functions; making it prop ready took me a good while, but it has given me much needed confidence on handling props in React now.  I'm also glad I took the time to do this, as placing multiple json files, and having alternative App.tsx files to pivot and accommodate through different data files is going to make this process so much smoother for tailoring or making content updates without altering the main codebase.   

------------

--- July 21st ---  
2025-07-21

This morning was mainly admin focused, so I used this afternoon to polish off my CV refactor project.  

Mostly content updates, but I also added an additional item in the content information section to include an additional link, and adjust the projects section styling; so the first bullet point from the list is removed and the styling is differentiated to slightly lift the project description outside of the responsibilities list.  

------------

--- July 22nd ---  
2025-07-22

Today I wanted to go back and look at where I left one of my personal projects at.  
  
It had been 3 months since my last content commit in WoC and honestly it took a while to re-familiarise myself with my milestones; what I wanted to achieve, and what my next steps are etc.  
It also made me realise that the repo was not easy to look at, not enough clarity was placed in some of my script naming conventions and the hierarchy just did not make enough sense.  The readme did not accurately reflect the pipelines either.  
  
So I spent this afternoon re-structuring the project, updating the pipelines so script outputs aligned with this new structure, and heavily updated the readme for more milestone clarity and emphasis on the ETL process.  

------------

--- July 24th ---  
2025-07-24

Yesterday I focused on small updates on multiple repos; mini content updates for my site, data additions for another, and adjusting readme files.  

Today I wanted to dive back into some studying, so completed the 2nd chapter of the 'Joining Data in SQL' course in Datacamp.  
This focused on outer joins (LEFT JOIN, RIGHT JOIN, and CROSS JOIN) and self join (which does not have it's own specific query name, but queries that allow joins to the same table using aliasing).  

Associate Data Engineer in SQL path - 38% complete.  

------------

--- July 28th ---  
2025-07-28

Today I wanted to focus and finish the 'Joining Data in SQL' course in Datacamp.  

So I paced myself, and managed to work through the final 2 chapters; this covered set types (UNION, INTERSECT and EXCEPT), anti-joins, and subqueries (from SELECT and WHERE).  
There was a lot to take on board and I'm thankful there were a lot of exercises to practice these new SQL keywords and queries.  

Associate Data Engineer in SQL path - 44% complete.  

I finished up the day with a little planning; finally creating a Github project for my portfolio site to track current issues & future improvements.  

------------

--- July 29th ---  
2025-07-29

After a full-on learning session yesterday, rather than continue the course, I wanted to practice and apply my current knowledge.  

So today I looked into completing the optional content; a project utilising a dataset to analyse international students' mental health.  
This was my first time utilising datacamp's datalab notebook environment, so I completed it's tutorial project to familiarise myself first.

I then moved onto the optional project: I enjoyed the exercise, practicing aggregation and aliasing, filtering, grouping and sorting the data. The only part I struggled with was successfully submitting the project itself - it was not obvious that I had to click on the table interface itself within the notebook to rename the Dataframe (I attempted with SQL keywords and a separate notebook for python logic before realising!). 

------------

--- July 30th ---  
2025-07-30

Today I wanted to continue my learning journey on Datacamp, so I made progress on 'Introduction to Relational Databases in SQL'.  

This is my second time looking at this topic, and I'm glad to say that this course is upping my level of understanding.  In this course I'm utilising a schema where we located a large table showcasing areas of redundancy, and then creating a new set of relational tables, preparing for data migration, migrating that data and dropping the original table.  
And that was just chapter 1. In chapter 2 I got to appreciate the usefulness of attribute constraints, changing types, and adding unique constraints.  I've also drawn up some Entity Relationship Diagrams for visual reference. I'm really enjoying this course so far.  

After a few hours of studying, I decided to move onto improving my portfolio site.  I've grabbed a few relevant tickets that I created in github projects the other day, opened a new branch to preview changes. 
  
I started with aligning the project image sizing within the carousel (for all different mobile views too), and then adding lazy loading on all images for performance improvements.  Despite a visual improvement from my former change, the latter has taken that down a notch.  
I've created an initial low res blur on first load for the carousel image, but does not help any later card switches. I am using transitions to help but it's not entirely removing the delay load-in of the image (although at least the card size appears to remain instead of bounce now).  
I also uploaded a webp file for my about me section, as my image was unnecessarily large - so the png now acts as a fallback, and appears to be working as intended. I am tempted to convert the project image files to webp too, however they are already alot smaller in size so it may not be noticeable.  

So I pushed the branch and viewed it in preview mode in vercel, however I will refrain from merging to main today in case there is any knock-ons I need to address asap.  

------------

<div align = "center"><i><a href="2025-05.md">May 2025</a></i></div>
