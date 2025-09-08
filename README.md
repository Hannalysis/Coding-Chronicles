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

<div align = "center"><a href="2025-08.md">August 2025</a></div>

