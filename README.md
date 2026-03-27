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

--- March 20th ---  
2026-03-20

To not lose momentum, I also spent this week on my personal figma to code project.  

I managed to complete two sections; one involving a carousel with a preview of the next one, and a creative layout of static images that are adjusted based on available width spacing.  

The Carousel component segment of this went smoother than expected. I was surprised that the preview of the upcoming carousel item view was doable by adjusting the parent Carousel container's overflow (hidden) and margin property (negative values), along with the usual flex and transform. This was also my fist time really getting a grip of utilising ternarys to toggle active and inactive states based on the current index, and therefore toggling their appropriate styling on the carousel indicators.  

I have noticed that the page is not behaving appropriately when shrinking down to smaller desktop widths overall, so that will be my focus later next week.

------------

--- March 27th ---  
2026-03-27

It's been a short week due to family commitments, however I did manage to make some progress in the last couple of days.  

As I mentioned in the last update, I decided to focus on making responsive layout adjustments for smaller desktops (1024px), and the mid point between that and the figma design at 1440px (1240px).  
There are 3 sections that are causing issues as soon as I shrink down from the design level, so after a while of trying to make wholesale changes, I opted for a component/section by section approach, and temporarily commented out those components to make the adjustments  on section content that was a bit more predictable.  With the red outline on, I managed to adjust grid and spacing ratios, and a bit of image clamping, and successfully made adjustments to the Layout (Header & Footer), and 3 of the 6 within the main section.  

One thing that was bothering me when testing responsive feedback on the web page using chrome devtools, is that the alignment of the page would often incorrectly shift. But I looked up any solutions and discovered a handy trick - pressing ctrl + 0 after clicking on the web page area resets the view. Granted, there are times when this does not work, but for the most part it improved my efficiency by quite a margin.  

------------

<div align = "center"><a href="2026-02.md">Feb 2026</a></div>
