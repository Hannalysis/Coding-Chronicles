<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> May 2025 </i></div>

 ------------

--- May 1st ---  
2025-05-01

As mentioned yesterday, I wanted to commence the Front-End Mentor challenge, the results-summary-component.  

I had no intentions to finish or rush to completion, but I am timing my progress for curiousity.  The reason I do not want to pressure myself for swiftness on this occasion, as I want to use this as an opportunity to really improve my code structure, and ensure it's clean and easy to read.  
I can revert to utilising prettier, however I've not set it automatically in hopes that I can train good behaviours for myself without over-relying on that tool.  
I also want to ensure I'm using appropriate element types inside the html (rather than just reverting to div at every opportunity).  

With 25 minutes of time allocated to just the planning process, this really helped me confirm how I wanted to containerise the component, what elements are best to use, and how it would be responsive from mobile to desktop.  
I decided to utilise the grid format; 1x2 for mobile, and 2x1 for desktop.  I also ensured the component was sitting in a main container, and the two containers within were using sections.  

After a bit of intial formatting on the results-container and its text content, including adding a gradient background to match the example, I decided to leave it there for today.

------------

--- May 5th ---  
2025-05-05 

After a bank-holiday break, I started my return to coding with some minor tweaks to my site.  This included deleting redundant comments, re-ordering my project carousel and adding additional tech stack icons, and adding additional meta tags.  

I then returned to working on the results-summary-component. 

I started witth curving the edge of the results component to make it look like it's overlapping the summary container space a little. I wasn't expecting the border radius to cause any issues, however you cannot simply add a linear-gradient to a border directly in CSS. So utilising my containers more efficiently, I moved the background styling and initial border radius of the results section into it's child container, and used the parent to simulate a border around that container, by using a background to behave like a border, and that way I could add the linear-gradient with no issue.  

I then added the circle gradient, the appropriate google fonts and formatting for the results section before moving onto my study session.  

I decided to return to my Data journey, and started the 'Foundations of PySpark' course with Datacamp, and completed the first chapter.  
I learnt the concept of how PySpark interacts by connecting to a cluster; creating an instance of the SparkContext class, and interacting with it by creating a SparkSession object.  From there, I learnt various commands to manipulate the SparkSession object to:  
  
Create an SQL query and show it, convert the query to a Pandas Dataframe, create a temporary instance of a conversion from a Pandas Dataframe to a SparkSession Dataframe - and then adding it back into the SparkSession's catalog properly, and storing a local csv to a SparkSession object.  

Course completion - 22%

------------

--- May 6th ---  
2025-05-06

Today I started by continuing studying the 'Foundations of PySpark'.  

The focus was to utilise data analysis techniques; by creating and modifying columns, filtering aggregating and joining data - by utilising both core Sparks methods, and pyspark.sql.functions for specific manipulation through columns. Course completion 49%.  

To allow time to digest my current learnings, I spent the remainder of time revising some FullStack fundamentals with codecademy exercises and best practices (mostly in HTML).  

------------

--- May 7th ---  
2025-05-07

Today I returned to work a little bit on the results-summary-component.  

I got the results section into a place I was happy with - by finally finding the appropriate gradient for the circular score container: 

    radial-gradient(circle at center top,  hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0));

I didn't realise until today that you can name the shape or direction, and also where it stems from as one argument; so now the shading matches the design brief.  I then focused on making the section's padding rem instead of percentage based for more accurate sizing adaptations when resizing, and made the overall component render as a card when viewed in desktop mode.  

For the remainder of my session, I allocated some study time on 'Foundations of PySpark' and managed to complete chapter 3.  
This chapter was focused on the pyspark.ml module; and utilising the Transformer and Estimator classes.  
I went through the motions in a simulated environment where I joined the DataFrames (but first prepped by renaming the appropriate columns to avoid duplication) to create the initial model data, transformed data and adding appropriate columns for those, 
made the appropriate StringIndexer calls and OneHotEncoder calls to hold our features; and finally adding everything into a VectorAssembler and making a Pipeline. I then finished up by transforming and splitting the data using randomSplit() to create a Test and Train set.  

It was an intensive study session, especially as I'm still quite green when it comes to the machine learning models at this stage. 80% Complete. Looking forward to seeing how the final chapter wraps up this course.  

------------

--- May 8th ---  
2025-05-08

Today I was eager to complete the 'Foundations of PySpark' course.  

I managed to succeed in this, and completed the final chapter - which introduced me to logistic regression for predicting binary outcomes. I learnt that the closer the model's AUC (Area Under the Curve) is to 1, the better the model is.  

So I went through the process of creating a modeler > evaluating it with a BinaryClassificationEvaluator with an ROC (Receiver Operating Curve) metric > making a grid & adding the hyperparameters > fitting the models with cross validation > and finally the evaluation by using the model to predict the test set.  

There's alot here I would like to investigate further, but I'm very grateful for studying this course - even though my primary goal was to focus on manipulating data it's also given me a taste of the pyspark.ml module, which could prove useful for my WoC data project when I approach the (later) machine learning stages.  

------------

--- May 10th ---  
2025-05-10

Just a short session today; I wanted to make most of the weekend and go for a long walk!  

So I spent time revisiting Flask, and revising my previous knowledge on the fundamentals.  

One thing I discovered today that was kind of irrelevant to the area itself, is that I only just found out that you can hold shift and click the refresh button on Chrome to perform a hard reload (so it re-fetches the previously cached web files).  I've not always encountered this issue when running in dev mode, but I have seen it occur enough to want to have known this little tidbit.

------------

--- May 11th ---  
2025-05-11

Another shorter session today - spent tinkering with Flask. 

In my playground project, I created more routes, used Jinja to create dynamic updates by injecting logic into certain templates, and utilised a couple of free external API calls.

------------

--- May 18th ---  
2025-05-18

I'm now pretty busy with my current contract, so updates will be less frequent. Ideally, I'll try and log once a week - no matter how small :)  

So today I started with something I really wanted to help speed me up in the long term - to create a template to showcase multiple groups of csv logs, to multiple dataframes in streamlit.  
Utilising appropriate file structure (I realise, I can be a bit lazy in Python compared to working with JS or TS so I need to create better habits) I created a repo to do just that. It's still a little bit specific, but I'm hoping the repo may grow into multiple streamlit templates that will aid a quick visualisation of small sets of data when I need them.  

I then ended my session by continuing on with my results-summary-component FE Mentor challenge. I managed to implement the summary icons, format the summary container with a bit of flex grow, and enforcing flex shrink on the button to pull it to the bottom to match the desired design.  I also had to create more containers to pair up the icons and type name, and the scoring so I could utilise the space-between css property value to give the middle of the container rows appropriate spacing.  
I also improved the mobile viewport by ensuring 100vh on the min-height property of the biggest container, meaning I could omit the footer on mobile but retain it on desktop to mimic the intended states set by the challenge.  

------------

--- May 24th ---  
2025-05-24

Today I wanted to return my attention to my focus on Data.  

Eager to re-solidify my foundations and revising some of the materials I had covered so far in recent courses I've completed in Datacamp, I wanted to start a Data Engineer career path - namely, the one focused in Python.  
However, it recommended I complete the 'Associate Data Engineer in SQL' career path before starting that track, and considering I wanted to really check I am comfortable with the fundamentals, it would be amiss for me to skip this career track.  

So I spent today completing the first section 'Understanding Data Engineering', which encompassed all 3 chapters.  This covered basic elements including the Data workflow and the requirement of data pipelines, how engineers process data and the benefits & risks of parallel computing.  
Course completion: 11%.  

------------

--- May 26th ---  
2025-05-26

It's a bank holiday, but I wanted to make sure I'm still making tracks so I decided to continue the 'Associate Data Engineer in SQL' career path.  

I completed the next section, the 'Introduction to SQL' fairly swiftly (thanks to previous knowledge; however I did pick up on a couple of points I'd forgotten or not realised: I'd forgotten that the DISTINCT keyword exists to pick up unique entries, and embarassingly did not realise that field naming conventions should always be singular.)  
  
So I decided to carry on with the next section, the 'Intermediate SQL' course. From there, I managed to complete the first chapter, which encompassed best practices when writing selections, and exercises to practice writing selections with a combination of COUNT, DISTINCT and aliases (AS).  
Course completion: 24%.  

------------

--- May 31st ---  
2025-05-31

Today I realised it was a good time to update my CV project, and add new experience (and certs I had not listed).  I also realised the main branch within this project, was so redundant from my Data branch that I decided to merge it over today, and worry about re-inserting the appropriate content after - so I dealt with my first github file conflict.  

I then finished my session by continuing my current career path in Datacamp, and therefore, continuing the 'Intermediate SQL' course.  I focused on a bunch of filtering queries, utilising a combination of operators, OR, AND, and BETWEEN | LIKE, NOT LIKE (% to match many characters, _ to match one in a specific part of the string) IN and NULL keywords.  
I managed to complete that chapter. Overall course completion thus far: 28%.  

------------

<div align = "center"><i><a href="2025-04.md">April 2025</a></i></div>
