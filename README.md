<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> March 2026 </i></div>

 ------------

--- March 6th ---  
2026-03-06

A very productive week! From two projects; two Layout systems now have a fully visual Header and Footer that matches the figma designs!  

Monday I'd almost finished the footer on my personal project; it was a fun challenge as I'd not really actioned on more than a basic footer - this one is akin to many business or commercial websites, with columns of subheaders, brand logo, user input for newsletter signups etc.  
That was also the day I'd learnt the use of adding the non-breaking space character into my work. I needed text into a subheader that did not exist in a particular column, so the appropriate space was created for the list of links that populate below it.  

For the remainder of the week, I focused my efforts on the relic colab project.  I implemented the grid, restricted and wide container classes, then moved onto a separate PR for the Header & Footer styling work.  
This is also the first time I ran into an issue where if you do not specify any content for a particular grid column (because we have nothing in that column on the figma) the browser will stretch columns automatically. So now I understand the use case of 
minmax(0, 1fr) in:  

    grid-template-columns: repeat(12, minmax(0, 1fr));

------------

--- March 13th ---  
2026-03-13

I've spent this week primarily focusing on my personal figma to code project.  

I completed two sections of the landing page, one was pretty straightforward thankfully, as the second one required more detail. The second section not only did I need to create a dynamic generation of product cards (of images and content), I also needed to implement an optional sticker, using chained ternary to select whether it's a sale or a new item (the sale amount is a property within the product object).  
And of course, both sections needed to match the figma designs on desktop so it was ensuring I was creating sensible design tokens, spacing and appropriate Typography classes for reusable content.  

Outside of this, I managed to complete the certification exams on Codecademy for the 'Improving Styling with CSS' as part of the Front End Engineer career path.  
Last but not least, I also reviewed an initial implementation of the localStorage system the relic colab project will be utilising, and I'm looking forward to implementing the next design section.  

------------

<div align = "center"><a href="2026-02.md">Feb 2026</a></div>
