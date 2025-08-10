<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> August 2025 </i></div>

 ------------

--- August 1st ---  
2025-08-01

Today I needed a bit of a palette cleanser, so I decided to go back Front End mentor, and continue the results-summary-component challenge.  

It didn't take me long to refamiliarise myself with where I'd got to and how the styling was working due to the container naming conventions I'd used.  I managed to complete the summary section of the component, which included colouring and spacing each sub section and utilising CSS variables for readability.
The button implementation was not too bad apart from getting the size to align with the summary sub sections, until I created a container for the button and sub-sections only.  A few other bespoke tweaks for desktop versus mobile and it's in a good enough spot to deploy, so it's now hosted on [github pages](https://hannalysis.github.io/front-end-mentor-results-summary-component/). I intend make a few more adjustments (including making score adjustments dynamically with the data json file), other than that, my next priority is to get a thorough readme created for this exercise.

 ------------

--- August 4th ---  
2025-08-04

I spent yesterday telling myself I was only doing admin; so I created my readme for my results-summary-component challenge.  Then I looked at my initial FE Mentor challenge I'd attempted in January, and decided it was a good time to implement the mobile-design element of the challenge.  
 
What I was not expecting, is how difficult I found it to pull styling from implementing desktop first, into mobile (after getting accustommed to mobile-first). I thought I could just change the flex into a grid and other styling changes would be minor.  But I found I had a fair amount of redundant styling properties on the original implementation, and I hadn't yet heard of CSS custom properties so there were many adjustments to make. So much that it basically bled heavily into todays work!  

I did manage to get that all commited and pushed in a branch, alongside an updated readme, PR made and merged, and is live on [this github page](https://hannalysis.github.io/front-end-mentor-product-preview-card-component/).  

That left me a little bit of time to start my Datacamp course on 'Database Design'. I managed to complete the first chapter which covered OLTP & OLAPs and suggestions for when you'd utilise each processing approach, data types and data storages, and defining a data model.  

 ------------

--- August 6th ---  
2025-08-06

I started this morning actioning out some of my front-end admin tasks. This included creating a separate repo to host my completed FE Mentor challenges.  
Currently, it's basically held in a readme file, but I do intend to extend that to a live page (stack and deployment tbc).  
   
I then moved onto continuing the 'Database Design' course.  I managed to complete chapter 2, which involved snowflake schemas; how to query for multi-dimensional tables, and when they're better suited for use. This also introduced normalisation, and the multiple layers of that (from 1NF - 6NF). I practiced converting a table that did not qualify for 1NF, and gradually shaped it to 3NF.   
  
Associate Data Engineer in SQL course completion - 60%.  

------------

--- August 8th ---  
2025-08-08

Yesterday I practiced utilising simple motion animations in React. Outside of that it was a pretty heavy admin day, so I wanted to take today a little easier.  

So, with no expectations, I continued my Datacamp course in 'Database Design'.  I managed to complete chapter 3, which focused on views; creating, updating (inc permissions) and also the differences between materialised views and normal views, and under what situations each are typically used for.  

------------

--- August 9th ---  
2025-08-09

Today I was determined to finish the 'Database Design' course in Datacamp; so I completed the final chapter.  
  
This split the focus between creating and editing access role and groups, and creating partitions. It was rounded off with an overview of different DBMS, examples and the best scenarios for each use case.   
  
Associate Data Engineer in SQL course completion - 66%. 

------------

--- August 10th ---  
2025-08-10

Today I wanted to start thinking about my next plan of action for my WoC data project, before heading back into studying.  

I looked into my next milestone, to re-evaluate.  Even though I had it in mind that I do not intend to use the entire dataset to display in Folium, I did not really give myself ample time to consider how I would aggregate and show the data.  I am thinking about potentially enriching the data further, and adding region/county to each record - however this will be too slow to fill via an API call at this point with 5 mil entries, so downloading a local dataset to enrich with may be the optimal path.   
I also wanted to explore utilising data validation tooling and adding it as part of the CLI process I intend to implement.  

Then, I spent the afternoon working through the entirety of the 'Data Warehouse Concepts' course in Datacamp.  As it's an introductory course, it was a great refresher and revision exercise for me. However, I did appreciate the high level overview of data validation (considering my previous paragraph mentioning this) and data governance programs.   
  
Associate Data Engineer in SQL course completion - 77%.  

------------

<div align = "center"><i><a href="2025-07.md">July 2025</a></i></div>
