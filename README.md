<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> May 2025 </i></div>

 ------------

--- May 1st ---  
2025-05-01

As mentioned yesterday, I wanted to commence the Front-End Mentor challenge, the results-summary-component.  

I had no intentions to finish or rush to completion, but I am timing my progress for curiousity.  The reason I do not want to pressure myself for swiftness on this occasion, as I want to use this as an opportunity to really improve my code structure, and ensure it's clean and easy to read.  
I can revert to utilising prettier, however I've not set it automatically in hopes that I can train good behaviours for myself without over-relying on that tool.  
I also want to ensure I'm using appropriate element types inside the html (rather than just reverting to div at every opportunity).  

With 25 minutes of time allocated to just the planning process, this really helped me confirm how I wanted to containerise the component, what elements are best to use, and how it would be responsive from mobile to desktop.  
I decided to utilise the grid format; 1x2 for mobile, and 2x1 for desktop.  I also ensured the component was sitting in a main container, and the two containers within were using sections.  

After a bit of intial formatting on the results-container and its text content, including adding a gradient background to match the example, I decided to leave it there for today.

------------

--- May 5th ---  
2025-05-05 

After a bank-holiday break, I started my return to coding with some minor tweaks to my site.  This included deleting redundant comments, re-ordering my project carousel and adding additional tech stack icons, and adding additional meta tags.  

I then returned to working on the results-summary-component. 

I started witth curving the edge of the results component to make it look like it's overlapping the summary container space a little. I wasn't expecting the border radius to cause any issues, however you cannot simply add a linear-gradient to a border directly in CSS. So utilising my containers more efficiently, I moved the background styling and initial border radius of the results section into it's child container, and used the parent to simulate a border around that container, by using a background to behave like a border, and that way I could add the linear-gradient with no issue.  

I then added the circle gradient, the appropriate google fonts and formatting for the results section before moving onto my study session.  

I decided to return to my Data journey, and started the 'Foundations of PySpark' course with Datacamp, and completed the first chapter.  
I learnt the concept of how PySpark interacts by connecting to a cluster; creating an instance of the SparkContext class, and interacting with it by creating a SparkSession object.  From there, I learnt various commands to manipulate the SparkSession object to:  
  
Create an SQL query and show it, convert the query to a Pandas Dataframe, create a temporary instance of a conversion from a Pandas Dataframe to a SparkSession Dataframe - and then adding it back into the SparkSession's catalog properly, and storing a local csv to a SparkSession object.  

Course completion - 22%

------------

<div align = "center"><i><a href="2025-04.md">April 2025</a></i></div>
