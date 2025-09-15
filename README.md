<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> September 2025 </i></div>

 ------------

--- September 2nd ---  
2025-09-02

Today I'm feeling happy about opening a PR in the colab project, I just need to await a review from my comrade then main will have some functional content!  I also updated the documentation, including adding a component/file tree so we can both have a high level view of the flow within our React project.  

So this afternoon I returned my focus to the career track in Datacamp, 'Data Engineer in Python'.  I completed the last chapter of the 'Cleaning Data in Python' course, which had me focusing on exercises for comparing strings, utilising the thefuzz and recordlinkage libraries.  
I went through the motions of calculating similarities of strings, generating pairs, drawing comparisons and finally linking them back to the DataFrame.  
  
I then started the optional cleaning data project on Datacamp, where I split the data into 3 separate dataframes, and have managed to clean up the first one of 3.  I aim to continue and finish this exercise tomorrow morning.  

------------

--- September 3rd ---  
2025-09-03

After a bit of an admin morning, I got an update from my colab partner to inform me they've reviewed the PR and given me the go ahead to merge it.  I had a few follow-up tweaks and suggestions to refactor so I've added those to the task pool, and will intend to address those before our verbal catch-up early next week!  
Also, whilst I was already inside our Github project, I decided to tidy-up the tasks, and add a few bespoke labels for easy filtering.  
  
This had not left me much of an afternoon left, but I've managed to complete the cleaning data project on Datacamp. 
On one of the exercises, I was asked to pull the month and day columns from the original DataFrame and use datetime to generate a new column with the typical format YYYY-MM-DD.  However, the months were stored as partial names (ie 'Jun', 'Jul' etc) and I did not realise until today that the lowercase b in the following code: 

    df_campaign['last_contact_date'] = pd.to_datetime(
    '2022 ' + df['month'] + ' ' + df['day'].astype(str),
    format='%Y %b %d'
    )

...is specifically for the abbreviated version of the month name.  Upon further investigation, there's alot more of that in the datetime module (%a for abbreviated weekday, I% for the 12-hour clock (as opposed to %H for 24-hour), %p for am or pm, ...and more!)   
Everyday is a learning day, even with a module I've used semi-frequently!    
 

------------

--- September 4th ---  
2025-09-04

Today I returned to studying my Data Engineer in Python career track in Datacamp.  

I'm just over half-way through the 'Writing Efficient Python Code' course.  I spent time on numerous exercises comparing the differences in execution time and memory consumption differences on varying ways of executing the same resulting code output (utilising the line_profiler and memory_profiler packages).  
  
I was also introduced to the power of zip, Counter (from collections) and combinations (from itertools), and unpacking their resulting objects into readable lists.  
  
Data Engineer in Python - 53% complete.

------------

--- September 5th ---  
2025-09-05

Before continuing my studying, I decided to spent this morning making a couple of minor refactors inside the MultipleChoice component as per my reviewer's suggestion from the previous PR, and opened a new PR, which we can go through next week.  

Then I spent the rest of my allocated time finishing up the course on 'Writing Efficient Python Code' in Datacamp.  Utilising timeit, I was able to see how improving what's executed in loops can make a huge difference on execution time.  In summary, its good to place one-time calculations above the loop, and holistic conversions after.  
  
I was also introduced to the benefits of comparing data using sets rather than lists; and applying this with the use of intersection(), difference(), symmetric_difference() and union() datatype methods.  

------------

--- September 8th ---  
2025-09-08

This week I'm determined to make great strides through my current career track course in Datacamp, so that was my primary focus today.  

I managed to complete an entire course, 'Streamlined Data Ingestion with Pandas'.  In all fairness, at least two of the chapters were mostly recap and revision, due to the fact that we had covered some of these topics for importing and reading JSON, APIs and SQL in earlier courses in this track, and back in the Associate Data Engineer in SQL course.  
However, I can say I got a lot out of the 2nd chapter, which was focused on excel data.  I'm still fairly green at processing excel sheets with pandas (partly due to the fact that I usually convert the excel files to other formats first!).  So I learnt how to select particular column ranges, sheet selections, and setting custom bool values - all with the pd.read_excel() function.  

Data Engineer in Python - 64% complete.  

------------

--- September 9th ---  
2025-09-09

Keeping inline with yesterday's statement, I've made good on my word to continue focusing my studying with Datacamp.  

I got a bit lucky regarding today's progress as I blitzed through two courses on Git alone, and 3 chapters of 'Software Engineering Principles in Python'.  One interesting takeaway from the latter course, is that there is a library that checks and outputs messages to inform whether the file/s code is PEP 8 compliant.  
  
This is pycodestyle; I did many exercises utilising this and I'm looking forward to utilise this library to check against some of my older ongoing projects.  

I ended the day with a lovely follow-up chat with my colab regarding our quiz project, and we've agreed on a couple of major tasks each to help us get our MVP in good stead. Really looking forward to making tracks on it again! 

------------

--- September 10th ---  
2025-09-10

Not feeling my best today, but managed to continue making strides in my studying.  

I managed to complete the last chapter of the 'Software Principles in Python course', and it's follow-up mini-project exercise of improving multiple functions utilising the PEP8 and DRY principles.  
  
I also started making progress on the 'ETL and ELT in Python' course, completed the first chapter which felt more like a recap and akin to previous data pipeline courses I've studied prior within Datacamp.  

Data Engineer in Python - 86% complete.  

------------

--- September 11th ---  
2025-09-11

Feeling more on form today, and I managed to complete the 'ETL and ELT in Python' course! One more course to go until the track is complete.  

Once again, I felt that there was a lot of overlap on this particular course, from other courses on this track as well as from the Associate Data Engineer track.  One thing that did stand out to me, was my introduction to @pytest.fixture, during the validation of data pipelines segment.  
They actually behave in a similar fashion to a decorator, and allows more modular coding practices as well as the reusability of the functions within a testing script.  

Outside of that, I did many exercises on reading in different file types to load into a local database - this was also my first encounter with the parquet file type (similar to csv, but processes faster).  

Data Engineer in Python - 92% complete. 

------------

--- September 12th ---  
2025-09-12 

I spent today working through the 'Introduction to Apache Airflow in Python' course, and managed to complete it! 

Definately did not breeze through this one, as it is a new tech and it was refreshing to get to grips with it.  I learnt about defining a DAG, multiple different Operators, scheduling tasks, branching together tasks, and creating templated commands.  
I'm looking forward to utilising Airflow as part of my CLI process in my current data project, WoC.  
  
Also, thanks to the course I was indirectly introduced to the cron syntax as an option for creating a schedule with as opposed to presets.  

Therefore, now I can say...  

Data Engineer in Python - 100% complete!!!  

Next week: More project focused!

------------

--- September 15th ---  
2025-09-15

I'm finding it hard to believe it's already been a month since my last commit for my data project, WoC. Today, that changes :) 

After re-familiarising myself with where I had left the project, I wanted to still finish the work I had started on the initial querying and visualisation branch. However, that still allowed me to make some refactors and adjustments!  
First and foremost I decided to utilise the sqlalchemy module (in addition to just psycopg) for a cleaner implementation for querying. I then created a function that saves the query into a local csv (to be visualisation ready), which I abstracted away into a utils folder to implement in a modular fashion thanks to the sys module.  

This also made me realise that some of my hard coded directory links for a lot of my code would not be useful if the project were to move to other devices/other people were to download it.  So I utilised the pathlib module to start swapping them out with something more concrete and unified so any pc setup may run it.  

All in all, I ended up pushing mostly chore and refactor commits outside of the first query result, however this puts me in a good position to do the visualisation work tomorrow.  

------------

<div align = "center"><a href="2025-08.md">August 2025</a></div>

