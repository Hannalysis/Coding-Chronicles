<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> October 2025 </i></div>

 ------------

--- October 2nd ---  
2025-10-02

I've been spending today creating a script to locally update my db with more accurate geodata for my data project, WoC.  

I started with psycopg and utilising a temporary table for my updated csv data to save to before making an update, however, upon debugging no matter what I did, after copying to this temp table, it was always empty.  
It contained data beforehand, and I had ensured I'd reset the buffer before actioning the copy, ensuring I'm actioning everything in a single connection, but after a few hours I decided to try creating an update script with sqlalchemy instead.  
After some minor struggles, it worked like a charm and I'm so glad I created this 'alt' script.  I also learned that utilising the begin() and connect() commands automatically uses commit or close commands, so I do not have to write them separately.  

My local database still had a couple of location entries that were invalid for my dataset, so I used a couple of SQL DELETE queries and updated my sweep 1 document accordingly.  Thankfully, my ETL has been updated so it would no longer seed non-UK entries otherwise I would have created it as part of a cleaning script.  
Tomorrow, I'll run the hopefully final data validation test - and merge my database update branch.  

------------

--- October 13th ---  
2025-10-13

After successfully running the data validation tests for WoC, I was able to merge the branch into main that Friday before last. After that I decided I required a much needed break, so I took last week off to relax and re-energise. 

Today I created my coding plans for the month, and after a quick update on my WoC readme (I'd forgotten to update my data validation tables to match the new figures) I decided to turn my eyes onto something new.  

I've been very curious about developing in Unity for awhile (especially integrating with Wwise), so I wanted to gently delve into some C#.  
I say gently partially due to the fact that it took longer than I expected to get VS Code to recognise the dotnet SDK (pathing issues!). Thankfully, installing and getting C# up and running in Visual Studio was painless.  

Once I'd insured both DE's were able to run very basic programs, I started to turn my attention to the intro in C# course in Codecademy so I can familiarise myself with the syntax differences from the languages I am familiar with.  

My main takeaway from that today is that the typings for handling numerical values have 3 options; float (not great), double (more precise than float, fastest execution times) and decimal (most precise).  Additionally, when setting a value to either decimal or float a trailing character is required at the end for float (f), or decimal (m).
Double can use d but it's assumed automatically.  

Intro to C# progress - 60% complete. 

------------

--- October 15th ---  
2025-10-15

Yesterday, I managed to complete the remainder of the Intro to C# course with ease (as it was only the basics).  
I could have continued into a more extensive course, but as Unity has it's own syntax too I've decided to set up Unity this morning, and go for the 'just in time' approach for this learning adventure!  

However, realising it had been a while since I made any progress on the colab project, I decided to branch off and start the round 1 styling.  
I thought I had made decent progress even with the basics (gradient background, fonts, and global styling variables). However I noticed when running the 'preview' instead of 'dev' (in React) my backgrounds were just black.  
  
Additionally, I attempted to utilise separate backgrounds for round one (depending on generation selection). Due to the fact our temp game selector return button is outside of the round component I'm styling, I was unable to make a fully covered background without making the styling a global change.    
  
I attempted a useEffect to add and remove classes to the body (as that would cover the whole screen) to no avail.  I'm going to park this for today and resolve these issues next time I'm on it.  

------------

<div align = "center"><a href="2025-09.md">September 2025</a></div>

