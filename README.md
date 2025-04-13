<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> April 2025 </i></div>

 ------------

--- April 1st ---  
2025-04-01

After a full day of designing, and a limited timeframe, I wanted to utilise AI to help me build the foundations of this site. However, the one I rely on will not allow for further prompts until 2 days time. Not great timing. So I opted to try a different one.  
Unfortunately, I was disappointed with the alternative, as despite carefully crafting an essay prompt, the AI only implemented each component one at a time, and it costed me a message to agree for it to create the new component.  And I'm looking at the results for what I have so far, thinking, it's alot to edit.  

Doable of course, but not in a day (not to a degree where's its demoable). Time frame aside now, this may develop into a side project of it's own, and be a foundation for improving my motion animation skills in the near future instead.  

With that in mind, I decided to end the day with two pomodoro's of 'Learning TypeScript'. I've now completed the section on type narrowing, and using examples of type guarding with if / else or if and simply return statements. 86% Complete.

------------ 

--- April 3rd ---  
2025-04-03

After a day or so of focusing on my CV and job focus, I decided to come back to learning some coding fundamentals today.  

So I decided to finish my 'Learning TypeScript' course in Codecademy, which focused on advanced object typing. This included optional type members, and the implements and extends keywords for class creation.  
Overall, this section was not as difficult as I thought it would be. It feels good to have the course completed, as it drew my attention to an area of TypeScript I am struggling with: complex types. So this will be great to take a note of, to revisit at some point.  

After that, I ended the day by adding content to my Continued Learning section of my portfolio site, and decided to add a couple of meta tags to my index. Unfortunately the og: image is not rendering at an appropriate size, so I'll look into fixing that next time I look at my site.  

------------ 

--- April 4th ---  
2025-04-04

Today, I decided to get back to my data analysis project, Winds of Change.  

After a brief re-familiarisation with the code, and adjusting the columns I'd like to view for the dataframe (and making sure I did not edit the folium data with a column it wasn't expecting...so it would still render); I started to make a plan regarding the data I have.  
Just shy of 3 million entries of weather data, in a CSV file. Placing that in my drive to convert to a google sheet, outright did not work as there was just too much information. So I spent a decent amount of time investigating my options to break down the CSV.  

I initially got a bit tunnel-visioned into the idea of utilising google's app script, however, even though it would solve my problem quite easily, it's not a great use case if my data was particularly sensitive, so I wanted to try alternatives. Then I realised something:  
Couldn't I manipulate my data utilising the panda dataframes, and converting it back to CSV? Turns out, I could! So I used that to filter only the columns I wanted and stored that to a new variable, and used the to_csv() function, which halved the size of the file.  
I tested this reduced CSV file and, after a couple of minutes, successfully converted this to a google sheet (for personal visibility, and the ability to analyse what data would be useful for seeding into a database).  

So this was progress, and I may want to use this to further cut/chunk down the CSV file (especially as the google sheet takes a considerable amount of time to load) next depending on whether I intended to only focus on recent/specific years of data.   

------------ 

--- April 6th ---  
2025-04-06

I had a bit of a false start yesterday - started to research into some ideas for my colab project, and then I managed to tweak my knee after a lovely morning walk.  

So, with resting and a cold compresses inbetween, I've managed to get a fairly productive day at the design table today. Did plenty of game and anime UI inspiration, and tried to keep it simple, especially due to the limitations of mobile-first.  
The biggest challenge I'm having so far, is being comfortable with using very bold primary colourings in my first draft - as I wanted the first iteration to remain on brand as much as possible.  Colours aside, I'm happy with the UI choices thus far, and managed to make a mock up for round 1 for both mobile and desktop versions. 

The next challenge of this project, is to see if I can make a home page that suits this visual theme, and try my ideas on a different generation (which utilises different but equally striking colour variants).  

------------ 

--- April 8th ---  
2025-04-08

Not feeling my best today, but after a doctors appointment this afternoon, I decided to have a bit of a researching & problem solving afternoon with my Winds of Change project.  
  
For starters, I wanted a separate google sheet with only the locations and no duplications. Simple enough to execute, was a little time consuming on execution no thanks to some forced revert on google cloud's end as it was struggling to save changes (likely due to the large file size).  
Then I needed to find an autonomous way to grab the lat and long of each of these UK locations, without having to utilise a payment method on an API-based solution.  There were numerous solutions, provided I had the postcodes at hand, and as I did not, I only had a couple of angles I could approach it from.  

At least this way, I believe I have found a method to grab both the lat long & postcodes both, provided I can get the script to execute successfully. Unfortunately, it's only executing manually at the moment, so I will look into this more next time.   
As a nice side note though, I was able to stringify and comma the entires within the google sheet using the formula ie ="'"&A2&"', ". This made it simple to copy and paste every town entry into a Python list inside the localised script file.  

------------ 

--- April 9th ---  
2025-04-09

I started this morning by continuing the wireframing on my colab project.  

I wanted to try out the same design idea with a different gen, which had more difficult colouring (Gen 6, A dirty blue w/ bold and swift gradient at the 50% mark to black (same with Red)).  Once settling with creating a slighly less aggressive fade, later (so it only takes just under 33%, and the first 25% is black - so UI is easier to distinguish), I decided that gradient effect needed to also be gently placed around the UI elements that touch the existing gradient and it makes it pop out better overall. 

So now, I'm looking at it, prefering it over the original bold colourings from the gen 1 design - despite really only testing this gen as I thought it would be more tricky, and therefore not a doable design at all thematically speaking. The gradients really make this wireframe look a bit more alive, and give it more character.  Looking forward to experimenting more with this.  

I then spent this afternoon back with my data project, Winds of Change.  After a brief look into alternative solutions, I actually managed to get my API fetch script call working - I just needed to add a user-agent property inside the header parameters.  With a 2 second wait between calls, the script took a hefty 17 minutes to execute.  

Once I looked at the saved csv file, there were 17 (out of ~500 locations) data unaccounted for, so I needed a method to quickly showcase the location names that did not successfully return any info.  So I utilised this google sheet formula (=FILTER(A2:A, ISERROR(MATCH(A2:A, B2:B, 0))) to quickly compare and showcase that location list, against the original list.  

So, my last task for today was to investigate these locations via a google map search, edit the names that were mostly not correct, cross off a couple of locations that did not seem to populate on google maps, and manually grabbed the geo data for entires that seemed fine but the API call did not manage. 

------------ 

--- April 11th ---  
2025-04-11

Today I was feeling quite revitalised and ready to continue the colab project, especially after I finally got round to completing the story of pokemon violet (it was worth it!). 

So I spent today creating the wireframe for the quiz homepage, for both mobile and desktop.  I decided to partially re-use the multiple choice UI selections I had made for the silhouette round to occupy the previous gen selection spaces. I then created bespoke areas for the current gen, an increased difficulty selection, and of course the start option.  I also decided to re-use the pokeball stencil as part of the start UI, which looks great in the wireframe - however I'm not sure how well that will translate to the actual build, once we get to it! 

Still, very happy with the progress today, only really missing what the selected options would/could look like, but I will leave that for another day.  

------------ 

--- April 12th ---  
2025-04-12

Today I decided to shift to researching on tech stacks I've heard of for a particular role I'm interested in; but not really had an initial overiew or known a comparative tech stack I have experience with.    
  
I started with learning about AWS Kinesis (A suite of services designed for real-time processing and analysis of streaming data at scale), Databricks DLT (a framework for building reliable, maintainable and testable data pipelines), and Microsoft Fabric (Data Management and analytics platform that simplies Data ingestion, transformation, storage and analytics). I also realised that SQL server is a variant of another RDBMS, which was much easier to grasp as I already have experience in postgreSQL.   
  
I then took a first look at PySpark, and revisted elements of data privacy and data security protocols.  

------------ 

--- April 13th ---  
2025-04-13

Today I returned to my data project, winds-of-change, to see if I could get as far as seeding the csv files into a local instance of postgreSQL.  
  
Firstly, I still had to grab those geo location data from a few that had been missed from the API fetch script. With those grabbed, and added to the appropriate csv location file, I needed to figure out the nuances between using python with pg vs node/javascript.  
Once I realised I required the Psycopg module (version 3), I realised it was very similar to the pg module (thankfully!) I started with creating my database instance inside pgAdmin, and created my tables there: 

    CREATE TABLE locations (
        location_id SERIAL PRIMARY KEY,
        location_name TEXT UNIQUE NOT NULL,
        latitude FLOAT,
        longitude FLOAT
    );
    
    CREATE TABLE wind_data (
        id SERIAL PRIMARY KEY,
        location_id INT NOT NULL REFERENCES locations(location_id),
        date DATE NOT NULL,
        wind_speed FLOAT
    );

I'm placing this SQL query here for a couple of reasons; one to remind myself to place this within the readme installation instructions, until I preferably, add this as part of the seed script file (I'm not sure why I didn't!).  
I started to run my seed script and quickly realised I still had inconsistencies with a few of my location names, so I addressed some of them with the following logic:

    locations_df['location_name'] = locations_df['location_name'].astype(str).str.strip()
    wind_df['location_name'] = wind_df['location_name'].astype(str).str.strip()  

and made some bulk replacements with a couple of oddities outside of that.  
Then I was ready to run the script! After a few minutes, the db had successfully populated both tables with the appropriate data! I ran a quick join query within pgAdmin to ensure the foreign key relationship was behaving as intended.  

I will need to make some more thorough data checks and queries to ensure it's validity, but that can wait until next time.  
  
I finished off the day by giving the readme a much needed update, and created a bespoke requirements.txt file (I did not realise that was the equivalent for nodes package json file).  Very pleased with my progress today!    

------------ 

<div align = "center"><i><a href="2025-03.md">March 2025</a></i></div>
