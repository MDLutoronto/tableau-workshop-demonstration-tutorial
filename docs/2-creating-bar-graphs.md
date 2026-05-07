
---
title: Creating Bar Graphs
parent: Tableau Workshop Demonstration Tutorial
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2022-08-31
nav_order: 2
---

## Creating Bar Graphs

1. We are going to start with a built-in dataset.  Under Saved Data Sources, select Sample - Superstore. <img src='{{ '/assets/images/TableauWorkshop1.1.jpg' | relative_url }}' alt='The Tableau home screen is shown with Sample – Superstore outlined with a red box at the bottom left' title='' width='1642' height='971' />
2. Let’s look around first before we dive in. On the left you can see Tables listed. Within a Table, the variables are listed, but divided by a thin grey line. Tableau categorizes variables as either Dimensions (above the line) or Measures (below the line). Dimensions are roughly qualitative data and Measures are roughly quantitative data.

    <img src='{{ '/assets/images/ReTableauWorkshop1-2.jpg' | relative_url }}' alt='Under the Tables menu on the left, Dimensions and Measures variables are outlined with a red box.' title='' width='1220' height='883' />
3. The centre area is where you’ll be dragging and dropping your variables on to different areas, such as Rows and Columns, or to vary Marks like Colour or Size by your variable, or filtering by a variable. Those areas that say Filters or Pages are called Shelves.

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.2.jpg' | relative_url }}' alt='The Pages and Filters boxes are outlined with a red box.' title='' width='896' height='576' />
4. The Marks area have what are called cards, and when the variables are showing up in those areas, they are called pills, as they are shaped like a pill. 

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.3.jpg' | relative_url }}' alt='The Marks area is outlined with a red box underneath the Pages and Filters boxes' title='' width='943' height='728' />  
    
    We’ll take a look at all these options as we go through the demo. One of the useful features of Tableau, to take a look at when you’re new to the tool and/or data visualization, is the Show Me feature. If you hold down Control and click on a couple of variables (hold down Command if on Mac), and then expand the Show Me tab, you’ll see that Tableau is giving you suggestions for what type of visualization to use.  

    <img src='{{ '/assets/images/TableauWorkshop1.2-2.jpg' | relative_url }}' alt='Order Date and Order ID are highlighted in blue and outlined with a red box under the Tables menu on the left. The Show Me menu is outlined with a red box on the top right' title='' width='1657' height='970' />
5. Okay, we’ve loaded in some data about a US fictional superstore, so let’s start by creating some visualizations that are used to make comparisons. Let’s start by making a simple bar graph. To keep track of all the visualizations we’re going to create, let’s rename our sheets as we go. Right-click on Sheet 1 at the bottom, select Rename, and give it the name “Sales Bar” and press Enter.

    <img src='{{ '/assets/images/ReTableauWorkshop1-3.jpg' | relative_url }}' alt='Sheet 1 at the bottom left and Rename from the pop-up menu are outlined with a red box' title='' width='' height='636' />
6. We’re going to create a horizontal bar graph to compare the amount of sales for different subcategories of products, with Sub-Category along the y-axis and Sales along the x-axis. Bar graphs are great for comparing categories. So drag the Sales variable (in the Measures section) next to Columns and Sub-Category (in the Dimensions section under Product) next to Rows.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-6.jpg' | relative_url }}' alt='A horizontal bar graph called Sales Bar is shown with Sub-Category along the y-axis and Sales along the x-axis. The Sales variable shown as SUM(Sales) is in the Columns and Sib-Category is in the Rows at the top' title='' width='1370' height='737' />
7. You can see that when we dragged Sales, Tableau automatically summarized it by adding up all the Sales values for each Sub-Category. Right now it is showing data combined for all of our States/Provinces, but let’s say we just want it to show one of them. We can filter by State/Provinces by dragging the State/Province variable (in the Dimensions section under Location) over to the Filters shelf and selecting one State/Province from the list.

    <img src='{{ '/assets/images/TableauWorkshop1.5.jpg' | relative_url }}' alt='State/Province is outlined with a red box under the Tables menu on the left, and Filters in the centre area is outlined with a red box' title='' width='1479' height='767' />  
        
    Let’s pick California in the pop-up window and click OK.

    <img src='{{ '/assets/images/ReTableauWorkshop1-5.2.jpg' | relative_url }}' alt='California is checked off and outlined with a red box. OK is outlined with a red box' title='' width='449' height='558' />
8. Now we have a bar graph showing the Sales by Sub-Category for California.

    <img src='{{ '/assets/images/ReTableauWorkshop1-6.jpg' | relative_url }}' alt='A horizontal bar graph showing the Sales by Sub-Category for California is displayed' title='' width='1370' height='737' />
9. Next let’s look at the Marks card. You can also see 5 smaller boxes labelled Colour, Size, Label, Detail, and Tooltip.

    <img src='{{ '/assets/images/ReTableauWorkshop1-7.1.jpg' | relative_url }}' alt='The Marks card with five smaller boxes underneath (color, size, label, detail, tooltip) in the centre area is outlined with a red box' title='' width='1293' height='765' />  
        If you click on Colour, you you can change the colour of the bars in the bar graph. Let’s pick a different shade of blue.

    <img src='{{ '/assets/images/ReTableauWorkshop1-7.2.jpg' | relative_url }}' alt='Color under the Marks card is outlined with a red box' title='' width='1126' height='673' />
10. We can also adjust the size/width of the bars using the Size slider.

    <img src='{{ '/assets/images/ReTableauWorkshop1-8.jpg' | relative_url }}' alt='Size under the Marks card is outlined with a red box. There is a size slider under Size' title='' width='1366' height='704' />
11. The Label section allows to create and customize labels. We can click on Show mark labels to see the values for each bar.

    <img src='{{ '/assets/images/ReTableauWorkshop1-9.1.jpg' | relative_url }}' alt='Label under the Marks card is outlined with a red box. Show mark labels is checked off and outlined with a red box' title='' width='1365' height='649' />  
        But you can see this makes our bar graph look cluttered, so let’s **keep Show mark labels unchecked.**

    <img src='{{ '/assets/images/ReTableauWorkshop1-9.2.jpg' | relative_url }}' alt='Label under the Marks card is outlined with a red box. Show mark labels is not checked off and outlined with a red box' title='' width='1380' height='657' />
12. You normally drag a variable on to the Detail section to expand out what’s plotted or visualized. We’ll look an example of this later.
13. Finally, the Tooltip section allows you to customize the text and format in the pop-up that shows up when you hover or click on a particular bar. For example, let’s add the broader Category that the product falls under in the Tooltip. To do this, drag the Category variable (in the Dimensions section under Product) to the Tooltip box.

    <img src='{{ '/assets/images/TableauWorkshop1.11-1.jpg' | relative_url }}' alt='Category under the Tables menu on the left is outlined with a red box. Tooltip under the Marks card is outlined with a red box' title='' width='1174' height='685' />  
        Then click on Tooltip. In the edit box, you’ll see that Category has been added underneath Sub-Category to the Tooltip. However, if you want to change the order, perhaps to have the broader category go first, you can click on Tooltip and edit the box. Let’s switch the order and click on OK.

    <img src='{{ '/assets/images/ReTableauWorkshop1-11.2.jpg' | relative_url }}' alt='OK is outlined with a red box in the Edit Tooltip menu' title='' width='548' height='409' />
14. As you can see there are options to customize a lot of parts of the visualization. You can also customize the axes. For example, right-click on your x-axis title, select Edit Axis...

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.1.jpg' | relative_url }}' alt='Edit Axis... is outlined with a red box near the x-axis of the horizontal bar graph' title='' width='1172' height='644' />

    Let's edit the x-axis Title to say 'Sales in US Dollars'. Then click the top right x button to close the pop-up.

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.2.jpg' | relative_url }}' alt='The X button at the top right and Sales in US Dollars Axis Title at the bottom left are outlined with a red box at the of the Edit Axis [Sales] General menu' title='' width='449' height='644' />
15. Right now the bars are sorted in alphabetical order by Sub-Category, but if you hover over the x-axis label, Sales in US Dollars, a small sort icon appears. Click on it to sort your bars by Sales instead. Every time you click the icon, it cycles through different sort orders. Let’s have it sort descending with the Sub-Category with the largest sales at the top. You can now easily see the top and bottom sub-categories in terms of sales.

    <img src='{{ '/assets/images/ReTableauWorkshop1-13.jpg' | relative_url }}' alt='The Sort Icon at the centre bottom of the horizontal bar graph is outlined with a red box' title='' width='1164' height='605' />
16. If we wanted to, we could also spread this visualization out a bit, so it isn’t squished up at the top. From the top ribbon where it says Standard, use the drop-down to select Entire View.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-14.jpg' | relative_url }}' alt='The drop-down menu from the top ribbon is outlined with a red box with Entire View highlighted' title='' width='1373' height='868' />
17. Finally, we can give our visualization a more meaningful title by double clicking where it says “Sales Bar” at the top. You’ll see the default title is the sheet name, but we can change that. Let’s put “Sales by Sub-Category for “ then instead of typing in “California”, we can make the title dynamic by click on Insert and selecting State/Province. Then if we change the filter, the title will automatically change. Now we’re done our first visualization!  

    <img src='{{ '/assets/images/ReTableauWorkshop1-15.jpg' | relative_url }}' alt='The Insert drop-down menu at the top right and State/Province near the bottom of the drop-down options are outlined with a red box' title='' width='658' height='495' />

 

### Creating Line Graphs

1. Okay, let’s create a new visualization. We need a new worksheet. Click on the New Worksheet icon at the bottom of the screen. Rename this one to “Line”.

    <img src='{{ '/assets/images/ReTableauWorkshop2-1.jpg' | relative_url }}' alt='The New Worksheet icon at the bottom right is outlined with a red box' title='' width='770' height='490' />
2. We’re going to create a line graph now, which is great to show trends over time. We’re going to create a line graph of change in total profit over time. Let’s drag Order Date variable (in the Dimensions section under Order) next to Columns. Next drag the Profit variable (in the Measures section) next to Rows. You’ll notice that our graph is summing Profit automatically.  

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
8. Right now it is showing the change in profit over time by years, but we can also change it to display more detail by quarters. One way to do this is to click on the plus sign next to the Year (Order Date) pill next to Columns. This subdivides each year by its quarters.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.jpg' | relative_url }}' alt='The plus sign next to the YEAR(Order Date) in columns at the top is outlined with a red box' title='' width='1095' height='623' />

    You might see a pattern of end of year growth, cycling over each year, depending on what sub-categories you have selected.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.2.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1238' height='830' />
9. Finally, let’s say you didn’t like these colours. Click on the Colour Box and select Edit Colours.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.1.jpg' | relative_url }}' alt='Color under the Marks card and Edit Colors... are outlined with red boxes' title='' width='779' height='637' />

    Here you can pick from a drop-down menu of various colour palettes. Select one you like and click on Assign Palette. Then click on OK.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.2A.jpg' | relative_url }}' alt='Tableau Classic 20, Assign Palette, and OK button are outlined with red boxes' title='' width='554' height='456' />
10. Again, give your graph a title “Quarterly Profit by Sub-Categories”. Lovely!

11. <img src='{{ '/assets/images/ReTableauWorkshop2-10.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1221' height='763' />

Technique: [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| Tools: [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)