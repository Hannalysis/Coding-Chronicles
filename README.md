<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> Februrary 2025 </i></div>

 ------------

--- Feb 1st ---  
2025-02-01

After finishing up the module from the bootcamp for this week, I wanted to take it easy after another intense week of React.  

I decided to branch off on our hackathon project, to fix a screen sizing issue that was occurring on one of my teammates' monitor.  With more freedom on the jsx files, I was able to manage the container layout, and centre everything appropriately, to give  
the header more space to move down (as it was clipping off on their screen). This should fix the issue, but it also made me realise I could add a media query so if the height was below a certain sizing on the viewport, it would disappear, giving the rest of our app  
more breathing space.  
  
After pushing that branch up to the remote repo; I realised I'd like to have those changes myself, so I forked the repo with that unmerged branch.  Which made me realise, I had no idea how to merge it manually, as the github website does not prompt a pull request on a forked repo  
with an unmerged branch. So I had to clone this forked repo, checkout the branch and ensure I had those changes locally, checkout main again, and then use the 'git merge branchname' command, and then push those changes back to the remote repo on main.  

------------ 

--- Feb 2nd ---  
2025-02-02

Same feeling as yesterday, I'm still winding down from a couple of intense weeks, so using today as a chill winding down coding session.  

I wanted to take the content of my CV (which I've been gradually updating in draft form) and transfer it to a fresh, modern template; therefore I've opened a repo and decided to design my own template.  
  
Revisiting my basic CSS skills, I managed to create a stylised header, and filled the basic wireframe for each section so far.  

------------ 

--- Feb 3rd ---  
2025-02-03

After an interesting day on User Centred Design; our team were focused on visual aid for progress and tracking, and it made me realise where I was in my current personal project (CoCo), afraid to delve into the next step and decide what data visualisation module to go for.  

So I got myself re-familiar from my previous research, and realised, even though I had my heart set on utilising a Python module - communicating the data from js and then sending the visuals back would require a back-end. That would give a noticable slowdown, and quite a time sink
considering this is just for my MVP, at this stage.  So, I rolled with the Plotly.js module, and created my bar range graph with PH data. It was not without teething issues. I did have to manually change the base property (as by default all bar graphs start at 0), and it turns out at my 'ranges',  
were simply adding the highest point as the amount to the lowest - so I had to make some logic to counter that.  Once that was resolved and the graph was generating inside the correct container with a button click, I committed my progress on that for the day.  
  
Following that, I had a quick investigation with star plots/radar charts in chart.js, to see if the team would be interested in utilising something like this for our visual progress tracker for our solution in this week's challenge.  

------------ 

--- Feb 4th ---  
2025-02-04

I wasn't feeling that well today, so I thought I'd try for a quick pomodoro session this evening, continuing on CoCo.  

So, I focused on trying to align the bar range graph better inside the container I'm placing it in, and also to align it with the instrument boxes on the left panel. The latter I did not manage today, but I was able to use the reverse function 
on all array data to ensure that the populated items were showing from top to bottom (instead of the opposite) to match the order of the items entered. I also got rid of all the margin space on the graph itself, for a better fit inside the container it resides in. 
Outside of that, I spent a good amount of time just reading through the plotly documentation, and watching a couple of YT vids on bar graphs (including animation frames, which I'd love to introduce at some point if required).

------------

--- Feb 5th ---  
2025-02-05

Today our bootcamp continued with our User Centred Design week with a focus on our storyboard, user journey, ethics discussions and user testing/feedback considerations.  
As it's another one of those intensive long days, I find myself usually struggling for energy on Wednesdays. After bringing this up with my mentor this evening, I realise my work/rest balance is not good enough, especially when I'm facing a topic I'm still struggling to 
get a full grasp of.  

So after a quick bug fix in last week's hackathon, Owlify (now all the incorrect multiple choice options have the chance to be any non-correct owl rather than just most of them), I will be taking the rest of this evening off to rest and recuperate.  

------------

--- Feb 6th ---  
2025-02-06

We spent today at SoC doing our first Design focused hackathon - utilising figma's prototype features.  
  
It is very useful in framing the visual side of a mobile application, with linking frames to imitate the touch user-flow experience that would be expected on a mobile application.  
What started as a simple 7 frame experience, turned into 22 frames, some of which, to behave in appropriate instances of the app, had to have some duplication to maintain a progressive feel during the app experience.

I would have finished up the day with a bit of coding practice, however I have some testing research lined up with a volunteer for today's hackathon prototype, so I'll need to document their responses and feedback their experiences to the team tomorrow in time for the presentation.

------------

--- Feb 8th ---  
2025-02-08

Due to the hectic week and after a great but tiring presentation day at SoC, I was unable to code yesterday evening.  

Today I got back to it! Returned to my CV creation (using HTML and CSS) - headers and PH font in, horizontal list items for Certifications created, and Personal Statement content added.  
I spent a bit more time in the Personal Information segment, as I needed to sort out the icons I wanted to use, and made sure they aligned appropriately using CSS nesting to avoid any duplication. 

------------

--- Feb 9th ---  
2025-02-09

Today I had to spend a lot of time working on my CV, as I have a meeting to discuss it tomorrow after bootcamp!  

So I got all the content added (that took most of my time today), which meant, unfortunately some of my formatting is not exactly how I want it, but it's close.  
I also spent some time researching into the modules I can utilise to convert my HTML & CSS into a decent pdf file.  
I ended up utilising one called Puppeteer, which, although its primary case used to be a web scraping tool, it has fell out of favour in comparison to other 
modules such as Playwright, and people tend to use this only for it's higher quality pdf conversion (compared to jspdf).  

------------

--- Feb 10th ---  
2025-02-10

Still feeling frazzled today; after our first day back at SoC starting on the DevOps module, I had a CV meeting scheduled striaght after.  

I got good feedback, and was hoping to implement all the minor tweaks and start trying to serve my projects post delving into some TypeScript, but unfortunately, I ran into a lot of online tech issues, namely being unable to sign up to netlify or vercel.  

------------

--- Feb 11th ---  
2025-02-11

Today at SoC we delved into Sentry, and as a team collectively work togather using a previous React project to get it running alongside it locally, and to force an error to occur to see how Sentry handles & visualises the information.  

After, I focused on tweaking my CV into a state I'm confident with.  Then I moved onto creating Readme files for the projects I wish to showcase with my future applications.  

------------

--- Feb 12th ---  
2025-02-12

Today at SoC we learnt about Github actions; in particular, the built-in secret scanning tool, and other open source security tool measures such as Trufflehog, that can be setup on push or pull requests to scan your file to check for sensitive data that could be accidently sent to the remote repo.  

Unfortunately, I did not feel well this afternoon, but I did manage to write a readme for the SQL hackathon, and serve our React Vite application using Vercel.  

------------

--- Feb 14th ---  
2025-02-14

Unfortunately I had to skip yesterday as I was being too poorly, especially by the evening.  

Today, after a much needed extended rest, I spent some time watching many tutorials on the Dev Ops cycle, ie IaC and the Infrastructure provisioning > Configuration of provisioned infrastructure > Deployment of app process.  
I also learnt how to utilise Docker, and some basic Github Actions.  

By the late evening, I started to feel like I had some energy to try something new, but perhaps not overly taxing - so I decided to create my first Next.js app, utilising Vercel's powerful AI design tool v0.dev, to create that initial setup file - with Typescript and Tailwind as the supporting tech stack.  
I asked for a basic Soundboard layout, with multiple buttons, and a random musician quote at the front and center (with a basic Header and Footer). Naturally, the sound part of the app did not function, as v0 is unable to grab source files, so I had to get that working myself.  

It took me some time to realise that not only did I require a custom.t.ds file (to allow Typescript to see a file locating to an .mp3 as an audio file), I also had to place the sounds folder inside the public folder, instead of the src folder 
(which is opposite to how React behaves).  It was a bit of a much-needed hurrah moment when I could hear sound in my Next application, and hopefully this reignition will further aid to my recovery.   

------------

--- Feb 15th ---  
2025-02-15

Today I had an opportunity for a dev to talk me through their recent interview technical test. It was so insightful; it was both reassuring to realise how much of it I could understand first-hand, while simultaneously, realising there's sections where I really do lack the knowledge right now.  

They were tasked with manipulating data from an SQLite table seeded with Employee names and Values. Outside of SQLite, their required techstack for this project was to utilise ASP.NET, React & TypeScript.  
They had to implement basic CRUD functionality to start with, then implement some custom specified queries that enforces the front end to update dynamically every time the data is modified.  
The dev showed off their form skills and implemented a form within a form, with a visual representation integrated as part of their table on their Front End experience. They also opted to implement test cases utilising Vitest to prove their implementation is robust.  

I then finished off the day with some exercises on TypeScript. I managed to convert a basic Rock, Paper Scissors js file into TypeScript, then made a 
basic web application using TS to fetch and display API data, using a tsconfig to convert TS to JS upon compilation.  

------------

--- Feb 16th ---  
2025-02-16

Today I continued with my Typescript Cardio exercise.  

I had to create a basic REST API utilising Typescript and Express. I had not actually delved into Express for a while, so it was a great return to practice those skills while also learning the nuances between making a backend with js Express instead of ts.  It was surprisingly similar, however the nuances were focused in the ts-node module, the tsconfig settings, and of course, not forgetting the type annotations, ie including Request, Response, and void names specified for controller functions.  

I took a break from Typescript to go back to the database hackathon utilising posgreSQL.  As my serving connection from Render has now expired, I wanted to re-configure the project to utilise a local connection.  It took me a little too long to realise that outside of the local string change, I also had to remove the SSL property from the index.js file (where we import the pg module).  

I also finally got some account functionality back with Codecademy after over a month of being unable to progress or start a new course. I used this opportunity to practice some Typescript and make a dent in the 'Learn Typescript' course; 13% complete.

------------

--- Feb 17th ---  
2025-02-17

New week at bootcamp, so new module! We were introduced to the Concepts of Cybersecurity, including how the Red and Blue teams operate, and more recently, the collaberation team known as the Purple team.  

After the lecture, I decided to continue my Typescript journey, and completed the Type module inside the 'Learn Typescript' course in Codecademy today; aka 22% complete.

------------

--- Feb 18th ---  
2025-02-18

Another day at bootcamp; learning about security and authorisation, followed by a group exercise to create a basic React App and utilise an Auth tool model - we picked Clerk and it was relatively straight forward to follow!  

After I completed the prep work, I continued my 'Learn Typecript' journey in Codecademy. I completed the Functions section, and learnt how to set an optional type parameter; you just need to use a question mark just after the argument name. 36% complete.

------------

--- Feb 19th ---  
2025-02-19

Today at SoC we did a hackathon-styled day, one day before our usual hackathon slot.  

Our task was to create a React App with Typescript, to utilise a weather API.  
My previous learnings of Typscript definately proved useful, although I still ran into some limitations - especially when we had to work out that we needed a conditional render on the API button that would only render the information if the fetch data was successful.  
Additionally, it was interesting to utilise a '|' optional typing for the fetch component in the instance that if a fetch was going to throw an error, Typescript can still expect an undefined as the alternative if the data is not fetched.  
We also had to on the spot show a 60 second demo to the cohort, so I put myself forward to do it; especially as I had navigated quite heavily on our solution today.  

------------

--- Feb 20th ---  
2025-02-20

Personal hackathon today; focused on creating an educational piece of content based around TypeScript, to present it in any format.  

So after a couple of hours researching into advanced features of TypeScript, I landed with TypeScript decorators - partly due to the fact that the concept isnt entirely unfamiliar to me due to my breif encounters with it in Python.  
I decided I wanted to make short thumbnail recording clips, and wrote two examples of pure TypeScript.  I was surprised how much time I spent just setting this up, there were a lot of steps.  

As for the solution type, I wanted to host this as a tutorial on a web-page, so practicing with the Next.js tech stack - especially as it's vercels go to.  

------------

--- Feb 21th ---  
2025-02-21

I managed to get the video content, and basic layout rendering as intended. However after learning how many steps it takes to successfully compile and run a pure TypeScript file, I decided to add an accordian component so when clicked, 
there is a list of instructions to set setup in VSCode. My version 0 was completed, and served up by vercel: content-hackathon.vercel.app.  

When we were sharing our hackathons with one another at bootcamp, one of my colleagues managed to stumble into a light mode only issue - turns out I had conflicting media queries setup! So I made that fix later that evening!  

And after that, that was me done for the day - I collapsed on the sofa for about 9 hours straight. But I'm not done with the app yet! As I mentioned in my social media post with this, I intended to make small incremental updates soon.

------------

--- Feb 22th ---  
2025-02-22

After finishing up with the course module from SoC, I decided to do some prep for next week's AI module.  

I delved into the Datacamp's free AI course for Prompt Engineering, and managed to complete it in 2 sessions.  I was surprised to learn about the prompt methods; especially the multi-shot tactic, md style for emphasis on certain words/phrasing for the focus in the response, 
and the ability to ask the AI if the information asked for is newer than it's cutoff point/last update, please reply with you do not know.  
It was also good to practice the SALT - Style, Audience, Length and Tone.  

After a decent rest, I decided to do a couple of pomodoro's worth of Learning Typescript in Codecademy, where I learnt how to set tuples ie:  
     
    let favoriteCoordinates: [number, number, string, number, number, string] = [40, 43.2, 'N', 73, 59.8, 'W'];

And I also learnt how to compare an element in Javascript to a particular typeof. 45% complete.

------------

--- Feb 23th ---  
2025-02-23  

I started this morning by looking at a side project plan, and writing some thoughts and risks for a particular feature.  

I then did a couple of Pomodoro sessions in the Learning TypeScript course in Codecademy. The difficulty is ramping up, and I already have alot of new concepts to digest, including:  
enums (including the stricter String variants!), object type annotations (both in function setting and variable assignment), Function Types, and Aliases.  
I particularly found the alias section interesting, because I could quickly see the appeal of avoiding duplication typing annotations, like with this example:  

    type Person = { name: string, age: number };
     let aCompany: {
       companyName: string, 
       boss: Person, 
       employees: Person[], 
       employeeOfTheMonth: Person,  
       moneyEarned: number
     };

------------

--- Feb 24th ---  
2025-02-24

Spent today at SoC on the topic centred around AI and data.  

Outside of that, I decided to do an audio and video version of my 2 TypeScript tutorials I made last week - which meant outside of going through the motions of the tutorial inside VSCode most of my time was spent inside wrestling with Openshot Editor, then Cubase.  

After a much-needed break, I finished the day by adding a couple of updates to my TypeScript Decorators tutorial - by adding proper mobile viewability, and adding a pointer cursor for the accordion component in desktop mode.  

------------
