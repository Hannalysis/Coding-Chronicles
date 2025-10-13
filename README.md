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

------------

<div align = "center"><a href="2025-09.md">September 2025</a></div>
