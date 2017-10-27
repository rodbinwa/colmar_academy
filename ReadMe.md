Capstone Project for CodeCademy's  Build Websites from Scratch

Project Name: Colmar Academy
Author: Rod Bray


The purpose of this project was to create a website for a fictitious company called Colmar Academy based on the specs located here:
https://s3.amazonaws.com/codecademy-content/courses/freelance-1/capstone-2/colmar-academy-spec.png

In the main directory you will find two files.
1. Index.html - This was created to fulfill the project specifications as indicated in the document referenced above.
2. Index-alt.html - This was created to use a different styling and some additional features such as transitions.

Both HTML files are almost identical.  I tweaked a couple of things on the -alt version to accommodate some of the styling ideas I had.  The whole project is built around nested flex containers.   I used the flex-basis functionality to set the width of different sections.

I limited the overall size of the page to 960px.  This seems to be a pretty standard size and was used on other CodeCademy projects.  I have three different pc/tablet sizes and a mobile device.  It rendered well on all screen sizes.

I used two large @media queries to build out the mobile and desktop sizes per the spec

<-- Header Section -->
The Header is built to stay at the top of the page and contains the log and navigational elements for both the desktop and mobile sizes.  The navigational elements are shown and hidden by the two media queries

<--  Main Container -->
This was put in only as a way to style each odd section of the page.

<-- Banner Section -->
The Banner has two main elements.  The 60% column with the image and the 40% column with the text and button.  As stated I used flex-basis to keep the sizes.  When the screen size changes I used different flex-directions to stack the elements on the smaller screen size.

<-- Announcements Section -->
I again used the flex basis to keep the sizes consistent with the Banner Section.  There is again a 60/40 split as shown in the spec.  Within the 40% column I used two additional flex items with the flex-basis set to 35% and 65%
For the smaller screen sizes, I used the @media query to hide the 60% column and stack the picture above the announcement text.  I used an nth-child styling to change the appearance of the third elements background.  In the -alt version, I used a hover property to highlight the item instead of keeping the third element highlighted.  
I learned in this section that you cannot nest anchor tags which through off some of my design ideas.

<-- Courses Section -->
Although not in the spec, I took some creative license and built the containers out of anchor tags.  I assumed this would be  links to additional information.  These items use the flex-wrap property to stack as the screen shrinks and grows.  using the @media query, I was able to change the appearance of the items  on mobile vs other sizes.

<-- Exhibits Section -->
This section is identical to the Banner Section.  The main call out is that in the spec the first item was highlighted.  I used the first-child pseudo class to highlight this item.  Again in the -alt version i made each item an anchor element and highlighted the item base on hover.


Thanks for taking a look at my project.  It was definitely a challenge but am happy at the results.

-Rod
