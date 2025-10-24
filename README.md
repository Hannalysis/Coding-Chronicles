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

--- October 16th ---  
2025-10-16

Today I first returned to the colab project, to resolve my issues from yesterday afternoon.  

I came back already realising my problem with the background not showing up at all on the preview build; the CSS variable was inside a modular CSS file that was not being utilised in it's relevant component file, so I had to move it.  This reminded me how important it is to npm run build & preview before committing changes.   

The second one was a bit more tricky. I discovered I could utilise prop drilling and grab the isolated button (which is not yet a bespoke component) into the round component, however, it would involve changing the logic of both files my comrade added recently, and it's far removed from my initial round 1 visual styling task.  
Therefore, I only refactored a file to added the ability to use modular css on that component, and used that to push the return button to the top of the page, giving me as much space as possible to style and continue my work.  

After testing, pushing and previewing the changes, I was pleased with the progress and decided it was a good time to switch it up.  So I spent the remainder of the afternoon going through the in-editor Unity tutorials.

------------

--- October 21st ---  
2025-10-21

It's been a few days of non-code specific learning. I started working through the Unity Essentials course on Friday as a wind down from a productive week.  
  
However, I ended up with joint pain and feeling under the weather over the weekend, so I kept it more lightweight this week so far. I started learning the basics of Tableau through Datacamps 'Data Analyst in Tableau' career track.  I do not have the intent to just push through all the content at once; I want to focus on the areas that will have the most direct use and impact for my data project for now, so I'm aiming for the Visualisations in Tableau course, which requires the intro and analytical courses to be completed first (all of which, are part of the track).  

Intro to Tableau - 51% complete.

I had a bit of time and energy after this, so I moved back onto my data project WoC, to branch of and begin adding pytests.  
I'm not sure why I started with the more challenging test (after adding the initial scaffolding); to mock the API fetch.  After adding the appropriate code and imports from unittest and the function in question, I realised the actual file code was running too (it was overwriting one of my processed data files!).  
Once I commented out the code from the original file in question, the tests were executing in question.  Then I realised I had not safe guarded the file itself, with: 

    if __name__ == "__main__":

I thought I understood this code, but it turns out I did not! So, wrapping this around my function block in the original file meant I could run the imported function with my mock code in isolation on the test file. 

------------

--- October 23rd ---  
2025-10-23

I completed the 'Intro to Tableau' course yesterday, so I wanted a bit of a palette cleanser before heading onto the next one.  

So I continued working on the styling of the colab quiz project; ensuring all the elements are now displayed in their appropriate locations, and focused on the multiple choice component styling - adhereing to the initial figma wireframes I created a while back.  
Today I realised two things:

1.  The CSS property 'background-color' is surprisingly restrictive; gradients have to be utilised within the 'background' property (much like images etc).
2.  Hexadecimal colour codes do use opacity; by adding two digits (numbers or letters) to the end of the original 6 digits. I used to defer to the rgba elements if I needed to change the transparency of something!

        Hex	Decimal	Opacity
        00	0	0% (transparent)
        1A	26	10%
        33	51	20%
        4D	77	30%
        66	102	40%
        80	128	50%
        99	153	60%
        B3	179	70%
        CC	204	80%
        E6	230	90%
        FF	255	100% (opaque)

I finished my session by starting the 'Analyzing Data in Tableau' course on Datacamp. I intend to complete the first chapter tomorrow morning.

------------

<div align = "center"><a href="2025-09.md">September 2025</a></div>

