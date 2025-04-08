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

------------ 
<div align = "center"><i><a href="2025-03.md">March 2025</a></i></div>
