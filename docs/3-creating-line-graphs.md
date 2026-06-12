---
title: Creating Line Graphs
parent: Tableau Workshop Demonstration Tutorial
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2022-08-31
nav_order: 3
---

### Creating Line Graphs

1. Okay, let’s create a new visualization. We need a new worksheet. Click on the New Worksheet icon at the bottom of the screen. Rename this one to “Line”.

    <img src='{{ '/assets/images/ReTableauWorkshop2-1.jpg' | relative_url }}' alt='The New Worksheet icon at the bottom right is outlined with a red box' title='' width='770' height='490' />
2. We’re going to create a line graph now, which is great to show trends over time. We’re going to create a line graph of change in total profit over time. Let’s drag Order Date variable (in the Dimensions section) next to Columns. Next drag the Profit variable (in the Measures section) next to Rows. You’ll notice that our graph is summing Profit automatically.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-2.jpg' | relative_url }}' alt='Order Date and Profit under the Tables menu are outlined with a red box. YEAR(Order Date) in Columns and SUM(Profit) in Rows above the line graph are outlined with a red box' title='' width='923' height='723' />
3. As we did before, from the drop-down at the top change it from Standard to Entire View.

    <img src='{{ '/assets/images/ReTableauWorkshop2-3.jpg' | relative_url }}' alt='The drop-down menu from the top ribbon is outlined with a red box with Entire View highlighted' title='' width='1357' height='908' />
4. It might be useful to see this graph broken down by Sub-Category – so basically adding a 3rd variable. The Sub-Category variable is just what it sounds like – a categorical variable, so we can assign different coloured lines for each category to display this information on the graph. To do this in Tableau, you drag Sub-Category (in the Dimensions section, under Product) on to Colour. 

    <img src='{{ '/assets/images/ReTableauWorkshop2-4.1.jpg' | relative_url }}' alt='Sub-Category under the Tables menu is outlined with a red box. Color under the Marks card is outlined with a red box' title='' width='1064' height='627' />  

    Tableau has assigned a qualitative colour palette scheme, assigning different colours to represent our Sub-Category, but we do have a lot of them, so it is a bit overwhelming.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-4.2.jpg' | relative_url }}' alt='Sub-Category at the top right of the line graph is outlined with a red box' title='' width='1223' height='763' />
5. When creating visualizations, you always need to figure out what your main message is. What is the story you are trying to tell. One way to simplify this would be to show a comparison between 2 particular sub-categories of interest. We can do this by dragging Sub-Category over to the Filters shelf.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.1.jpg' | relative_url }}' alt='Sub-Category under the Tables menu is outlined with a red box. Filters in the centre area is outlined with a red box' title='' width='960' height='612' /> 

    Select two sub-categories. Let’s pick Phones and Tables. (Select None first to clear the selections).  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.2.jpg' | relative_url }}' alt='Phones and Tables are checked off and outlined with red boxes. The None and OK buttons are outlined with red boxes' title='' width='444' height='556' />

    This tells a story that Phones are increasing in profit, while Tables are decreasing.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.3.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories (Phones and Tables) are displayed' title='' width='1202' height='761' />
6. Another way we could tell a story would be to allow the user to filter it themselves based on what sub-categories they are interested in – so adding an interactive element. To do that, go back to Filters shelf, right click on Sub-Category and pick Edit Filter. 

    <img src='{{ '/assets/images/ReTableauWorkshop2-6.1.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters is outlined with a red box. Edit Filter... from the Sub-Category menu is outlined with a red box' title='' width='752' height='558' />

    Select All and click on OK.  
        <img src='{{ '/assets/images/ReTableauWorkshop2-6.2.jpg' | relative_url }}' alt='All and OK buttons are outlined with a red box' title='' width='446' height='556' />

    Then right click Sub-Category in the Filters shelf again, but this time select Show Filter. Now you can see the Sub-Category filters show up on the right. We can select or deselect as we like and the graph changes. Or select (All) to have them all come back. (if you don’t see the filters, click on Show Me to close its options panel that is blocking the view)  

    <img src='{{ '/assets/images/ReTableauWorkshop2-6.3.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters on the top left is outlined with a red box. Show Filter from the Sub-Category menu is outlined with a red box. Sub-Category with checked categories is outlined with a red box at the top right beside the line graph' title='' width='1383' height='841' />
7. To further help the user read your graph, you could also add a Highlighter. Go back to the Filters shelf, right click on Sub-Category, but this time pick Show Highlighter.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-7.1.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters on the top left is outlined with a red box. Show Highlighter from the Sub-Category menu is outlined with a red box. Highlight Sub-Category to the right of the line graph is outlined with a red box' title='' width='1392' height='792' />  

    Now Highlight Sub-Category box shows up on the right. The user can pick a sub-category and the graph emphasizes that Sub-Category – try it out. You should see it emphasized on the graph.
    
    <img src='{{ '/assets/images/ReTableauWorkshop2-7.2A.jpg' | relative_url }}' alt='Highlight Sub-Category and Paper are outlined with a red box to the right of the line graph' title='' width='1230' height='655' />
8. Right now it is showing the change in profit over time by years, but we can also change it to display more detail, such as by quarters. One way to do this is to click on the plus sign next to the Year (Order Date) pill next to Columns. This subdivides each year by its quarters.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.jpg' | relative_url }}' alt='The plus sign next to the YEAR(Order Date) in columns at the top is outlined with a red box' title='' width='1095' height='623' />

    You might see a pattern of end of year growth, cycling over each year, depending on what sub-categories you have selected.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.2.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1238' height='830' />
9. Finally, let’s say you didn’t like these colours. Click on the Colour Box and select Edit Colours.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.1.jpg' | relative_url }}' alt='Color under the Marks card and Edit Colors... are outlined with red boxes' title='' width='779' height='637' />

    Here you can pick from a drop-down menu of various colour palettes. Select one you like and click on Assign Palette. Then click on OK.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.2A.jpg' | relative_url }}' alt='Tableau Classic 20, Assign Palette, and OK button are outlined with red boxes' title='' width='554' height='456' />
10. Again, give your graph the title “Quarterly Profit by Sub-Categories”. Lovely!

11. <img src='{{ '/assets/images/ReTableauWorkshop2-10.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1221' height='763' />

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)