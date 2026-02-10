<h1 align = "center"> Coding Chronicles </h1>
 <div align = "center"><i> January 2026 </i></div>

 ------------

--- Jan 10th ---  
2026-01-10

Turns out, that small cold evolved into a full-blown flu! Not my favourite start to the year, however I'm finally over the worst of it and ready to lightly get back to the coding journey :) 

After being recommended the Frontend Unicorn ebook (amongst many others!), I'm starting today with a nice chill reading session over most of the introductory sections.  
Going forward, my aim is to read 1 or 2 chapters to start my day before going into any practical learning or project sessions.  

Note: I seem to have not mentioned that I learnt what kerning is at some point during the festive period, so writing it here - the spacing between two letters in a text. Most typefaces are well-designed that it's not a concern, however it can be useful when for editing header or title text.  

------------

--- Jan 12th ---  
2026-01-12

I've continued my reading of Frontend Unicorn over the last couple of days, and I'm already 25% through.  
So I thought I would label a learning/takeaway from each of the recent sections:

DESIGN - 12 column web grids are the standard for desktop. This also allows to create sections on the site into the most possible broken down configurations (1,2,3,4 or 6 width of equal section widths). 

COLOURS - Avoid colours that are saturated over 90%. 

TYPOGRAPHY - Best shape for short centered text is a triangle. Single column forms are better for a single path to follow with your eyes.  

BUTTONS - At least 1W of padding for each side of a button label (best to go for 2xW).  Min size: 44x44 mobile | 32x32 desktop.

------------

--- Jan 14th ---  
2026-01-14

To keep expanding my data knowledge, I completed a high-level course yesterday on 'Marketing Analytics for Business' with Datacamp. This gave me an overview of campaign analysis, privacy implications, text analysis & forecasting requirements. 
As the course itself was a little dry, I also weaved in some front-end reading (which continued into today).  

And today, I updated my site - as I realised one of my continued learning cards was not displaying all information appropriately. Turns out, one of my entries within my data file utilised the incorrect name for a particular property within the 'course' type.  

Further takeaways from Frontend Unicorn (47% read):
- Loading states are better represented with skeleton screens
- Cut out icons require bounding boxes for ease of implementation
- Reasonable markup improves your search ranking
- Test focus states for keyboard only navigation

------------

--- Jan 18th ---  
2026-01-18

On Friday, I managed to get some follow-up feedback from the code review of my recent branch for my colab project (which, I will start to codename as Po-Qu as I will be starting another colab in the near future!).  
So that merge for mobile first styling is now in main (along with some much needed package updates!), and a session for further comms is pencilled in for the week after next; so I may have time to add additional commits to improve the desktop styling and potentially add in the reveal anim mechanic (as previously agreed upon).  

Though, the reason I'm really logging today as I've just managed to complete my first read-through of the Frontend Unicorn ebook.  
Here are some takeaways from the mobile section, which provided me with valuable insights:  
- In future products where I'd want to learn and utilise React Native, I should consider frameworks such as SwiftUI for a smoother transition from React syntax.
- If there is a radio button or checkbox, a user will assume they can also click the label to interact with it. Syntax example for setup:

      <input 
        type="checkbox" 
        id="option1"
      />
      <label for="option1">
       Option 1
      </label>
  
- Screen readers will benefit from the ARIA attribute role = "button" to force behaviour on non buttons, to behave like a button.
- If a clickable area looks small, it's best to use a larger invisible clickable area for the button, especially for mobile users.
- As hover only works on desktop, using a 'ripple' like effect will produce feedback of a similar natureon mobile.
- Everything that should be focusable: Links | Options & Menus | Buttons | Inputs | Text areas | Selects | Custom Pickers

I'm looking forward to leveraging these learnings to make improvements not only to my site and Po-Qu, but all my new projects going forward. Also, looking forward to getting my hands on more of the recommended reads and pick what area to focus on next! 

------------

--- Jan 23rd ---  
2026-01-23

It's been a very productive week!  

Monday, I started working on a new colab project - and we managed a full planning session on a Figjam board, hand drawn simple sketches of what our pages/views could look like, and decided what we wanted our app to focus on.  
Tuesday, I opened a joint repository and Github project to assign our first set of pre-production issues, we created our desired list of criteria for our MVP & supporting tech stack, and we created the final sketch for our first view. We also allocated a couple of areas of ownership, and I was honoured to be allocated product and design owner.  I will also be implementating the majority of feature areas of the front end so I'm very much looking forward to translating my figma wireframes into the resulting application.  

On Wednesday I wanted to turn my attention to the Po-Qu colab project, to continue working on the desktop styling implementation for round 1.  I made some good progress, however I noticed I was spending a lot of time checking out properties of grid.  
So I intentionally paused on that for the remainder of the day, and decided to setup the figma wireframe template for the desktop layout on the new colab project (going to refer to it as Relic from here on out), and add the Grid Layer (utilising the sensibilities taught from Frontend Unicorn; 12 columns, 24px gutter, 80px margin (and 8px gaps)).  I also learnt how to setup my nav and footer layers with the appropriate padding and wrapper layers.  

So Thursday was to be my learning day, and I spent it back on the Codecademy career path 'Front End Engineer'.  I happened to have stopped right at the introduction of the Grid layout, so I got stuck in and came out learning and understanding the various syntax and short-hand versions thereof.  
Interestingly, I also learnt that Grid layout can be known as Explicit or Implicit, and the one you use depends on the implementation you require.  If theres an unknown amount of entries that populate within an area, you'd create an Implicit Grid implementation so grid items fill up rows first, adding new rows as necessary and newly generated grid rows will only be tall enough to contain the content within them.  

After gaining some much needed grid knowledge I returned to the Po-Qu colab project today and managed to implement the grid section with more success. The elements and components are now aligned appropriately and move as one but remain entirely intact when the page is resized; it looks much better.  
After pushing up the branch changes remotely I returned to the Relic colab project and started work on wireframing the locations of the content for the MVP view.  

------------

<div align = "center"><a href="2025-12.md">Dec 2025</a></div>
