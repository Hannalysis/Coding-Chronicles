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

--- April 15th ---  
2025-04-15  

Today I decided to start learning and understanding the Databricks tech stack; which is a cloud-based data platform that unifies data engineering, analytics, and AI on a collaborative, scalable lakehouse architecture.  

I began an introductory course in Datacamp, which allows the me to utilise a sandbox environment of Databricks. Its helping me learn my way around the initial navigation and useful elements of the Databricks platform.  
I also learnt that a Control Plane is the 'brains' of the system, which is the user's Databricks account, and the Compute Plane, is the 'muscle' which is the user's AWS/Azure cloud services (aka the Databrick clusters). 40% complete.  

------------ 

--- April 22nd ---  
2025-04-22  

It's weird seeing my contributions squares with a row of black instead of my usual green; my first proper break since coding on github (and coding overall, minus a couple of days for Xmas).  

Much needed though; we finally got our full fibre installed, and much needed time travelling to visit some family.  Recharged and ready to get back to it 🙏   
  
I thought I'd start with a 'warm up' by adding media queries to the Owlify quiz project. Turns out, that was not as straightforward as it first seemed. Firstly, it's not using modular CSS and secondly the separation of concerns even within the two CSS files were not consistent.   
I've unified the selectors and placed them inside the appropriate two different CSS files that project contains, and media queried at the bottom of each. Interestingly, despite managing to successfully make the web app compatible with mobile devices, the end result is not behaving the same on the deployed site as my local dev enviornment.   

Not a big deal for now as it's very much playable (compared to before), however, there is some wobble and you're able to scroll after the background image which is unintended.   
  
I finished the day with continuing the 'Introduction to Databricks' course, where I learnt about the different kinds of data (structured, semi-structured and unstructured), Delta (open source storage format, fully ACID compliant, batch & streaming datasets), and serverless cluster types.   

I also created my first cluster utilising a local dataset on books, and created my first SQL and pySpark queries, using the Databricks Notebooks, and connecting my cluster to that particular notebook session. Course now 83% complete.  

------------ 

--- April 23rd ---  
2025-04-23

I started today by finishing up the 'Introduction to Databricks' course - and realising I had not really left myself much to do on that outside of recapping the previous chapters!

So I updated my 'Continued Learning' section on my portfolio site with the new certification. I am noticing that the timeline line is starting to misbehave the more I'm adding to it, so, I'm going to have to come up with a scalable solution in the future.  I also attempted to fix my og-image issue whilst I was at it, however this is going to take 
real life time to see whether it was successful.    

Still plenty more of Databricks to explore, but I'm going to leave it there for today and give myself a chance to absorb the information. So I spent the rest of my allocated time today on...  

My site: I thought it's about time I started planning my solution to my carousel implementation.  I spent some time looking at my two major areas of functionality that require addressing on the Projects section: the stability of the chevrons, and the images loading as they transition in.  
Once I looked into my options (and actively using figma to break it down into those two battle plans), I made a new branch and began working on the chevron issues.  Once I pulled the chevrons to a container I was able to fix them to, I was then able to freely fix the height of the carousel container itself.
This immediately brought stability to the chevrons when moving between different project card sizes. However, the chevron buttons themselves would overlap on various mobile sizes - as this is a mobile first app, I had to fix this before making any commits. So I spent a while making bespoke adjustements of the projact card sizes, and button spacing  
on about 5 separate media queries, as I wanted them to look good and still be easily viewable regardless of what device the user has.  

Then I commited and pushed my branch to my remote repo, and was pleasantly surprised that vercel offers a preview deployed link for branches (with no additional setup on my project), so I was able to test my changes in production with ease. I was not originally intending to merge my branch until I had both issues addressed, 
but this fix had already improved the functionality of the carousel over what currently exists on main it gave me the confidence to merge it straight away! Next time I will be taking a look at more graceful image loading.  

------------ 

--- April 24th ---  
2025-04-24  

Today I wanted to enjoy my progress with my site, without making any further adjustments so I'm returning to my data ventures.  

I decided to start a course on AWS Kinesis and Lambda, which notably had a fair amount of prerequisite courses recommended before delving in. However, I had a basic understanding of AWS, so I wanted to see how much I could learn and understand before having to visit a potential area/concept I was unsure of.  

Thankfully, the initial concepts did not feel as alien as I had expected; understanding use cases of batch vs streams is something I already had been introduced albeit at a higher level a while back, and the coding exercises and examples are all written in Python.  
I spent today learning about Firehose, and sending data to an Amazon S3 bucket.  I started with understanding and navigating through the AWS permissions flow and creating a role via the IAM (Identity Access Management). This was then followed up by creating the Firehose Delivery System, by:
- Locating the role ARN (Amazon's unique identifier)
- Initiating the boto3 client
- Creating the stream
- Creating the stream response
- Sending a record (and converting it to a string format)
- Waiting for buffering to complete for the data to be ready to view inside the S3 bucket
- Copy the key of the created file, and create an S3 client using boto3
- Get the object from S3 -> read the object into a Pandas Dataframe

It's alot to take in, so I did not quite finish the 1st of 4 chapters of this course today. However I will continue this tomorrow! 18% complete.

------------ 

--- April 25th ---  
2025-04-25  

Today I decided to spend my afternoon fully focused on continuing the datacamp course on 'Streaming Data with AWS Kinesis and Lambda'.  

It was intense for the most part, but I managed to finish chapter 1 and 2 of 4. The remainder of chapter 1 was practicing and reviewing creating the Firehose stream, creating the S3 bucket, and successfully sending a record to said bucket.  
Chapter 2 was all focused around Lambda; serverless code execution in the cloud, triggered by events.  I first covered the examples of when serverless is appropriate to utilise for certain data over manual servers, then moved onto creating lambda functions.  
The first function I created would trigger every time a record entered the bucket. I was then introduced to adding layers so we could utilise Pandas (so we can read the S3 files) by utilising the aws-data-wrangler.  I followed this up by creating a timed lambda function trigger, by adding a scheduler expression (with cron).  

This was thankfully followed up with an area I'm more familiar with, API creation.  Lambda makes this pretty straightforward using their functions - with the API Gateway trigger config. Course completion: 52%.    

------------ 

--- April 26th ---  
2025-04-26 

Today I wanted to continue working on the 'Streaming Data with AWS Kinesis and Lambda' course.  

It was focused on Lambda transformations and Kinesis Data Analytics. I learnt about the ability to utilise lambda functions to sanitise incoming Firehose stream data before it reaches the S3 bucket, and using Kinesis Data Analytics to join multiple streams, find anomalies along with discovery patterns (ie in a certain timeframe) with SQL.  

I took a lot of notes, to ensure I could navigate around the AWS services appropriately and ensure the setup would be correct in the particular testing scenario that is provided in this course.  
I also practiced writing Python scripts to encode incoming strings to bytes, then base64, and converting them back to bytes, and finally strings using the base64 module. Chapter 3 will be continued tomorrow - course progression 70% complete.  

I finished my allocated session today by deciding on a few Frontend Mentor challenges to commence. I've had quite a data focused month but I do not want to negate my front-end journey either.  I'm looking foward to interweaving them into my studying to keep things fresh.  
  
------------ 

--- April 27th ---  
2025-04-27

Today I wanted to continue studying the AWS course, but I needed a bit of a mental warm-up first.  

So I took a quick return to my TypeScript decorators tutorial page - the post I created on linkedin that links to the deployed site still has fragments of viewership and I find the website to be a little rough around the edges still.  
I decided to make some quick wins - created sleek thin borders around the grid items (both video and step info), aligned this with the header and summary sections and unified them visually, and gave a little more room for the accordion instructions component.  

Then I continued my learning journey with 'Streaming Data with AWS Kinesis and Lambda'. I managed to complete chapter 3, and started looking at alternatives to S3 for storing non-static data - so the focus was on setting up Elasticsearch as the destination of a newly created Firehose stream.  
This followed nicely into CloudWatch, which allows the viewing of raw logs, metrics, visualisation dashboards and alarms. I was then guided through the process of setting up an alarm when incoming record data to trigger under certain conditional criteria.  

Course completion - 89%. Let's see if we can finish it tomorrow!

------------ 

<div align = "center"><i><a href="2025-03.md">March 2025</a></i></div>
