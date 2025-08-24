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

--- August 11th ---  
2025-08-11

Today I wanted to see how far I could get in the next course on my career track on Datacamp.  

So I ended up completing the 'Introduction to Snowflake' course.  Outside of a couple of keyword deviations from postgreSQL, the majority of new clauses or functions I encountered are bespoke to Snowflake; including CAST, EXTRACT, GROUP BY ALL, CURRENT_DATE, and INITCAP().  I also got to practice utilising their additional join keywords, NATURAL and LATERAL.  I enjoyed using CTE to give a nickname or alias to a subquery for readability.  I was also introduced to Snowflake's QUERY HISTORY view, which displays useful metrics as such execution time; which gives insight to optimise slower running queries.  

All in all, very excited to learn more about Snowflake, and to study further in data engineering; especially as today is the day I have completed the 'Associate Data Engineer in SQL' career track course! A couple of optional projects to still complete, and I aim to do those soon to help solidify or revise my recent learnings.  

Associate Data Engineer in SQL course completion - 100%.  

------------

--- August 13th ---  
2025-08-13

Had to take yesterday off due to how toasty it was!  

I started today with a small content update to my site, then did some SQL practice with Datacamp.  I aim to start my next career track course next week, so I'm keeping my studying light in the meantime.  

I followed up with adding the dynamic data implementation for the results-summary-component FE Mentor challenge.  It was good javascript DOM practice and I also got to utilise github pages for the first time on a non-main branch due to mandatory testing to ensure the update was utilising the json file before merging it back to main.  

I ended the day by working on the initial API fetch and data storing for the colab project.  I ended up running into some issues as I had a node update since I last worked on this, causing numerous running issues until I had addressed through the config.  I also had to create a bespoke config so I could run the fetch in TypeScript.  However, I managed to get the data required for the quiz, so I pushed my changes to my new branch; will tidy up and utilise properly next.  

------------

--- August 14th ---  
2025-08-14

After a quick warm up with some review and practice with sub queries in SQL with Datacamp exercises, I decided it was time to create a new branch in my data WoC project and start investigating.  

So I focused on querying to answer a fairly straightforward question to start with, and make that the focus for the first exploration point: "What are the highest wind speeds available from this dataset?"  
I documented each query, from simply selecting everything from the wind_data table, joining it to the location table when I wanted more readability over ids, and realising I needed to add a subquery once I utilised the DISTINCT keyword on location names.   
  
Once my query had started to evolve, I noticed my execution times went from 0.5 to 7.5 seconds, then I moved a query around and it down to 0.1 sec!  At first I thought it was my window function, but then I saw I had also moved the wind speed filter.  
I looked into anything I could use to diagnose this, and discovered that there is a performance query in SQL to help: 
    
    EXPLAIN(ANALYZE, VERBOSE) 
   
When my WHERE clause for the wind speed was outside of the subquery I was only filtering ~400 records before the remainder of the query was executed, and when it was inside the subquery we managed to filter out over 900k records first.  I would go into it further, however I have the full query process located in my branch [here](https://github.com/Hannalysis/winds-of-change/blob/initial-explore-and-vis/explorations/highest-wind-speed/hws-query-process.md).  Next step is to visualise this before heading into the next exploration.  

------------

--- August 19th ---  
2025-08-19

After a lovely break seeing family I'm gearing myself to get back into the swings of things.   
  
I managed to complete the optional Data Analysis project on Exploring London's Travel Network, and thoroughly enjoyed creating the appropriate queries.  I followed this up with the optional skill test; thus completing every element of the career path in Datacamp.  
  
Before heading into the new career track today, I wanted to research and create a very rough game plan to consider an approach to learn another language, utilise my audio middleware knowledge and creating something to implement audio systems against, and of course, work out what areas of mathematics I'd need to learn to understand and implement some of those concepts.  
It's alot; and considering I already have a lot of goals regarding my software development it's going to have to be very focused sessions despite being very much on the back burner. Happy to have taken the very initial small step towards that today though! 
  
Finally, I started the Data Engineer in Python career path in Datacamp, and due to it's fairly straightforward introductory courses I'm already 11% complete. 

 ------------

 --- August 20th ---  
2025-08-20

Today I continued plowing through the content within the Data Engineer in Python career track in Datacamp, and managed to complete two courses.  

This is due to the fact it was mostly covering introductory Python topics such as functions, modules, error handling etc. However, I was pleased to be introduced to Docstrings (perhaps slightly embarassing that I had not come across this before!).   
This is useful when creating custom functions in Python, and can be accessed with the help() function, or more specifically, using dunders: 

    print( function_name.__doc__)

Data Engineer in Python - 21% complete.  

I finished off my session by returning to the colab project.  I started with refactoring the api fetch, and then did an initial commit displaying the imported pokemon images from the data file (post api call), which randomly generate from a button press (for now).  

------------

 --- August 23rd ---  
2025-08-23

Much like the last entry, today I continued my studying with Datacamp on the Data Engineer in Python career track.  

I managed to get through 2/3 's of the next course, which focused on importing numerous different file types.  It was my first time loading and extracting data with matlab files, pickled files, hdf5 files & sas and stata files.  Similar process, but slightly different syntax and execution, along with requiring certain libraries to assist (ie numpy, pandas and scipy).  Outside of file importing, I was also introduced to PEPs (aka Python Enhancement Proposals).  I am enjoying picking up these tidbits of information I just happened to miss out on when I initially started learning to code in Python.   

------------

 --- August 24th ---  
2025-08-24

I managed to finish the Introduction to Data Importing in Python, and the follow-up Intermediate course today! 

The intermediate course focused on packages I have experince in, including urllib, BeautifulSoup and of course requests - so I utilised the course as a revision and refresher excerise.    
What was interesting to me was the final chapter of the former course, where the focus was creating & connecting to the database engine, querying and then saving the results to a DataFrame. This was my first time utilising sqlite and sqlalchemy, however I did some additional research and found that I can utilise postgres modules in a similar way as long as I'm using the psycopg driver.  So it's directly useful for my data project, WoC.   

Data Engineer in Python - 35% complete.  

------------

<div align = "center"><a href="2025-07.md">July 2025</a></div>
