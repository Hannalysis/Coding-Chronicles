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
