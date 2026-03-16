---
title: "Tableau Workshop Demonstration Tutorial"
layout: "home"
description: "This tutorial outlines the steps taken in the demonstration during the live workshop on an Introduction to Data Visualization Using Tableau Desktop. This is a companion tutorial, but can also be used as a stand-alone introduction to Tableau Desktop."
permalink: "/"  #! Remove this if not the homepage
staff:
 - name: Kelly Schultz
   link: https://library.utoronto.ca/staff/kelly-schultz
---

# Tableau Workshop Demonstration Tutorial

This tutorial outlines the steps taken in the demonstration during the live workshop on an Introduction to Data Visualization Using Tableau Desktop. This is a companion tutorial, but can also be used as a stand\-alone introduction to Tableau Desktop.

## Set Up and Starting Up

1. Download the 3 example dataset Excel files and save them somewhere on your computer where you can find them, such as your Desktop:
	* [AuthorDataCitationGrants.xlsx](https://maps.library.utoronto.ca/workshops/Tableau2022/AuthorDataCitationsGrants.xlsx)
	* [AuthorDataExperience.xlsx](https://maps.library.utoronto.ca/workshops/Tableau2022/AuthorDataExperience.xlsx)
	* [RomeoAndJulietWordFrequenciesByAct.xlsx](https://maps.library.utoronto.ca/workshops/Tableau2022/RomeoAndJulietWordFrequenciesByAct.xlsx)

2. Open up Tableau Desktop (tutorial uses version 2022\.2\).

## Creating Bar Graphs

1. We are going to start with a built\-in dataset.  Under Saved Data Sources, select Sample \- Superstore. <img src='{{ '/assets/images/TableauWorkshop1.1.jpg' | relative_url }}' alt='The Tableau home screen is shown with Sample – Superstore outlined with a red box at the bottom left' title='' width='1642' height='971' />
2. Let’s look around first before we dive in. On the left you can see Tables listed. Within a Table, the variables are listed, but divided by a thin grey line. Tableau categorizes variables as either Dimensions (above the line) or Measures (below the line). Dimensions are roughly qualitative data and Measures are roughly quantitative data.

    <img src='{{ '/assets/images/ReTableauWorkshop1-2.jpg' | relative_url }}' alt='Under the Tables menu on the left, Dimensions and Measures variables are outlined with a red box.' title='' width='1220' height='883' />
3. The centre area is where you’ll be dragging and dropping your variables on to different areas, such as Rows and Columns, or to vary Marks like Colour or Size by your variable, or filtering by a variable. Those areas that say Filters or Pages are called Shelves.

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.2.jpg' | relative_url }}' alt='The Pages and Filters boxes are outlined with a red box.' title='' width='896' height='576' />
4. The Marks area have what are called cards, and when the variables are showing up in those areas, they are called pills, as they are shaped like a pill. 

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.3.jpg' | relative_url }}' alt='The Marks area is outlined with a red box underneath the Pages and Filters boxes' title='' width='943' height='728' />  
    
    We’ll take a look at all these options as we go through the demo. One of the useful features of Tableau, to take a look at when you’re new to the tool and/or data visualization, is the Show Me feature. If you hold down Control and click on a couple of variables (hold down Command if on Mac), and then expand the Show Me tab, you’ll see that Tableau is giving you suggestions for what type of visualization to use.  

    <img src='{{ '/assets/images/TableauWorkshop1.2-2.jpg' | relative_url }}' alt='Order Date and Order ID are highlighted in blue and outlined with a red box under the Tables menu on the left. The Show Me menu is outlined with a red box on the top right' title='' width='1657' height='970' />
5. Okay, we’ve loaded in some data about a US fictional superstore, so let’s start by creating some visualizations that are used to make comparisons. Let’s start by making a simple bar graph. To keep track of all the visualizations we’re going to create, let’s rename our sheets as we go. Right\-click on Sheet 1 at the bottom, select Rename, and give it the name “Sales Bar” and press Enter.

    <img src='{{ '/assets/images/ReTableauWorkshop1-3.jpg' | relative_url }}' alt='Sheet 1 at the bottom left and Rename from the pop-up menu are outlined with a red box' title='' width='' height='636' />
6. We’re going to create a horizontal bar graph to compare the amount of sales for different subcategories of products, with Sub\-Category along the y\-axis and Sales along the x\-axis. Bar graphs are great for comparing categories. So drag the Sales variable (in the Measures section) next to Columns and Sub\-Category (in the Dimensions section under Product) next to Rows.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-6.jpg' | relative_url }}' alt='A horizontal bar graph called Sales Bar is shown with Sub-Category along the y-axis and Sales along the x-axis. The Sales variable shown as SUM(Sales) is in the Columns and Sib-Category is in the Rows at the top' title='' width='1370' height='737' />
7. You can see that when we dragged Sales, Tableau automatically summarized it by adding up all the Sales values for each Sub\-Category. Right now it is showing data combined for all of our States/Provinces, but let’s say we just want it to show one of them. We can filter by State/Provinces by dragging the State/Province variable (in the Dimensions section under Location) over to the Filters shelf and selecting one State/Province from the list.

    <img src='{{ '/assets/images/TableauWorkshop1.5.jpg' | relative_url }}' alt='State/Province is outlined with a red box under the Tables menu on the left, and Filters in the centre area is outlined with a red box' title='' width='1479' height='767' />  
        
    Let’s pick California in the pop\-up window and click OK.

    <img src='{{ '/assets/images/ReTableauWorkshop1-5.2.jpg' | relative_url }}' alt='California is checked off and outlined with a red box. OK is outlined with a red box' title='' width='449' height='558' />
8. Now we have a bar graph showing the Sales by Sub\-Category for California.

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
13. Finally, the Tooltip section allows you to customize the text and format in the pop\-up that shows up when you hover or click on a particular bar. For example, let’s add the broader Category that the product falls under in the Tooltip. To do this, drag the Category variable (in the Dimensions section under Product) to the Tooltip box.

    <img src='{{ '/assets/images/TableauWorkshop1.11-1.jpg' | relative_url }}' alt='Category under the Tables menu on the left is outlined with a red box. Tooltip under the Marks card is outlined with a red box' title='' width='1174' height='685' />  
        Then click on Tooltip. In the edit box, you’ll see that Category has been added underneath Sub\-Category to the Tooltip. However, if you want to change the order, perhaps to have the broader category go first, you can click on Tooltip and edit the box. Let’s switch the order and click on OK.

    <img src='{{ '/assets/images/ReTableauWorkshop1-11.2.jpg' | relative_url }}' alt='OK is outlined with a red box in the Edit Tooltip menu' title='' width='548' height='409' />
14. As you can see there are options to customize a lot of parts of the visualization. You can also customize the axes. For example, right\-click on your x\-axis title, select Edit Axis...

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.1.jpg' | relative_url }}' alt='Edit Axis... is outlined with a red box near the x-axis of the horizontal bar graph' title='' width='1172' height='644' />

    Let's edit the x\-axis Title to say 'Sales in US Dollars'. Then click the top right x button to close the pop\-up.

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.2.jpg' | relative_url }}' alt='The X button at the top right and Sales in US Dollars Axis Title at the bottom left are outlined with a red box at the of the Edit Axis [Sales] General menu' title='' width='449' height='644' />
15. Right now the bars are sorted in alphabetical order by Sub\-Category, but if you hover over the x\-axis label, Sales in US Dollars, a small sort icon appears. Click on it to sort your bars by Sales instead. Every time you click the icon, it cycles through different sort orders. Let’s have it sort descending with the Sub\-Category with the largest sales at the top. You can now easily see the top and bottom sub\-categories in terms of sales.

    <img src='{{ '/assets/images/ReTableauWorkshop1-13.jpg' | relative_url }}' alt='The Sort Icon at the centre bottom of the horizontal bar graph is outlined with a red box' title='' width='1164' height='605' />
16. If we wanted to, we could also spread this visualization out a bit, so it isn’t squished up at the top. From the top ribbon where it says Standard, use the drop\-down to select Entire View.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-14.jpg' | relative_url }}' alt='The drop-down menu from the top ribbon is outlined with a red box with Entire View highlighted' title='' width='1373' height='868' />
17. Finally, we can give our visualization a more meaningful title by double clicking where it says “Sales Bar” at the top. You’ll see the default title is the sheet name, but we can change that. Let’s put “Sales by Sub\-Category for “ then instead of typing in “California”, we can make the title dynamic by click on Insert and selecting State/Province. Then if we change the filter, the title will automatically change. Now we’re done our first visualization!  

    <img src='{{ '/assets/images/ReTableauWorkshop1-15.jpg' | relative_url }}' alt='The Insert drop-down menu at the top right and State/Province near the bottom of the drop-down options are outlined with a red box' title='' width='658' height='495' />

 

### Creating Line Graphs

1. Okay, let’s create a new visualization. We need a new worksheet. Click on the New Worksheet icon at the bottom of the screen. Rename this one to “Line”.

    <img src='{{ '/assets/images/ReTableauWorkshop2-1.jpg' | relative_url }}' alt='The New Worksheet icon at the bottom right is outlined with a red box' title='' width='770' height='490' />
2. We’re going to create a line graph now, which is great to show trends over time. We’re going to create a line graph of change in total profit over time. Let’s drag Order Date variable (in the Dimensions section under Order) next to Columns. Next drag the Profit variable (in the Measures section) next to Rows. You’ll notice that our graph is summing Profit automatically.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-2.jpg' | relative_url }}' alt='Order Date and Profit under the Tables menu are outlined with a red box. YEAR(Order Date) in Columns and SUM(Profit) in Rows above the line graph are outlined with a red box' title='' width='923' height='723' />
3. As we did before, from the drop\-down at the top change it from Standard to Entire View.

    <img src='{{ '/assets/images/ReTableauWorkshop2-3.jpg' | relative_url }}' alt='The drop-down menu from the top ribbon is outlined with a red box with Entire View highlighted' title='' width='1357' height='908' />
4. It might be useful to see this graph broken down by Sub\-Category – so basically adding a 3rd variable. The Sub\-Category variable is just what it sounds like – a categorical variable, so we can assign different coloured lines for each category to display this information on the graph. To do this in Tableau, you drag Sub\-Category (in the Dimensions section, under Product) on to Colour. 

    <img src='{{ '/assets/images/ReTableauWorkshop2-4.1.jpg' | relative_url }}' alt='Sub-Category under the Tables menu is outlined with a red box. Color under the Marks card is outlined with a red box' title='' width='1064' height='627' />  

    Tableau has assigned a qualitative colour palette scheme, assigning different colours to represent our Sub\-Category, but we do have a lot of them, so it is a bit overwhelming.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-4.2.jpg' | relative_url }}' alt='Sub-Category at the top right of the line graph is outlined with a red box' title='' width='1223' height='763' />
5. When creating visualizations, you always need to figure out what your main message is. What is the story you are trying to tell. One way to simplify this would be to show a comparison between 2 particular sub\-categories of interest. We can do this by dragging Sub\-Category over to the Filters shelf.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.1.jpg' | relative_url }}' alt='Sub-Category under the Tables menu is outlined with a red box. Filters in the centre area is outlined with a red box' title='' width='960' height='612' /> 

    Select two sub\-categories. Let’s pick Phones and Tables. (Select None first to clear the selections).  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.2.jpg' | relative_url }}' alt='Phones and Tables are checked off and outlined with red boxes. The None and OK buttons are outlined with red boxes' title='' width='444' height='556' />

    This tells a story that Phones are increasing in profit, while Tables are decreasing.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-5.3.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories (Phones and Tables) are displayed' title='' width='1202' height='761' />
6. Another way we could tell a story would be to allow the user to filter it themselves based on what sub\-categories they are interested in – so adding an interactive element. To do that, go back to Filters shelf, right click on Sub\-Category and pick Edit Filter. 

    <img src='{{ '/assets/images/ReTableauWorkshop2-6.1.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters is outlined with a red box. Edit Filter... from the Sub-Category menu is outlined with a red box' title='' width='752' height='558' />

    Select All and click on OK.  
        <img src='{{ '/assets/images/ReTableauWorkshop2-6.2.jpg' | relative_url }}' alt='All and OK buttons are outlined with a red box' title='' width='446' height='556' />

    Then right click Sub\-Category in the Filters shelf again, but this time select Show Filter. Now you can see the Sub\-Category filters show up on the right. We can select or deselect as we like and the graph changes. Or select (All) to have them all come back. (if you don’t see the filters, click on Show Me to close its options panel that is blocking the view)  

    <img src='{{ '/assets/images/ReTableauWorkshop2-6.3.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters on the top left is outlined with a red box. Show Filter from the Sub-Category menu is outlined with a red box. Sub-Category with checked categories is outlined with a red box at the top right beside the line graph' title='' width='1383' height='841' />
7. To further help the user read your graph, you could also add a Highlighter. Go back to the Filters shelf, right click on Sub\-Category, but this time pick Show Highlighter.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-7.1.jpg' | relative_url }}' alt='The Sub-Category drop-down under Filters on the top left is outlined with a red box. Show Highlighter from the Sub-Category menu is outlined with a red box. Highlight Sub-Category to the right of the line graph is outlined with a red box' title='' width='1392' height='792' />  

    Now Highlight Sub\-Category box shows up on the right. The user can pick a sub\-category and the graph emphasizes that Sub\-Category – try it out. You should see it emphasized on the graph.
    
    <img src='{{ '/assets/images/ReTableauWorkshop2-7.2A.jpg' | relative_url }}' alt='Highlight Sub-Category and Paper are outlined with a red box to the right of the line graph' title='' width='1230' height='655' />
8. Right now it is showing the change in profit over time by years, but we can also change it to display more detail by quarters. One way to do this is to click on the plus sign next to the Year (Order Date) pill next to Columns. This subdivides each year by its quarters.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.jpg' | relative_url }}' alt='The plus sign next to the YEAR(Order Date) in columns at the top is outlined with a red box' title='' width='1095' height='623' />

    You might see a pattern of end of year growth, cycling over each year, depending on what sub\-categories you have selected.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-8.2.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1238' height='830' />
9. Finally, let’s say you didn’t like these colours. Click on the Colour Box and select Edit Colours.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.1.jpg' | relative_url }}' alt='Color under the Marks card and Edit Colors... are outlined with red boxes' title='' width='779' height='637' />

    Here you can pick from a drop\-down menu of various colour palettes. Select one you like and click on Assign Palette. Then click on OK.  

    <img src='{{ '/assets/images/ReTableauWorkshop2-9.2A.jpg' | relative_url }}' alt='Tableau Classic 20, Assign Palette, and OK button are outlined with red boxes' title='' width='554' height='456' />
10. Again, give your graph a title “Quarterly Profit by Sub\-Categories”. Lovely!

11. <img src='{{ '/assets/images/ReTableauWorkshop2-10.jpg' | relative_url }}' alt='Quarterly Profit by Sub-Categories bar line graph is shown' title='' width='1221' height='763' />

 

## Creating Pie Charts

1. Let’s try loading our own data – this time some qualitative humanities data. Tableau is not meant to work directly with text data files, but you can use other better\-suited textual analysis tools to create datasets that you can then visualize in Tableau. What I did was take the freely available text for Shakespeare’s play Romeo and Juliet. I ran it through a free online tool called [Voyant Tools](https://voyant-tools.org/) and it generated a word frequency table that we are now going to use as our dataset. If you want to learn more about textual analysis and visualization tools, such as Voyant, you can take a look at the [Tools & Tutorials page](https://mdl.library.utoronto.ca/dataviz/tools-tutorials) in the [data viz guide](https://mdl.library.utoronto.ca/dataviz/getting-started).  

    <img src='{{ '/assets/images/ReTableauWorkshop3-1.jpg' | relative_url }}' alt='Voyant home screen is shown' title='' width='1004' height='521' />
2. Let’s load this word frequency data into Tableau. Again, go to Data\-\>New Data Source.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-2.1.jpg' | relative_url }}' alt='In Tableau, Data and New Data Source are outlined with red boxes at the top left' title='' width='958' height='651' />  

    Select Microsoft Excel.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-2.2.jpg' | relative_url }}' alt='Microsoft Excel outlined with a red box in the Connect menu' title='' width='1121' height='765' />  

    Pick RomeoAndJulietWordFrequenciesByAct.xls. in your folder.  

    <img src='{{ '/assets/images/ReReTableauWorkshop3-2.3.jpg' | relative_url }}' alt='RomeoAndJulietWordFrequenciesByAct.xls outlined with a red box' title='' width='1022' height='612' />
3. You can see that it is a simple spreadsheet that counts how many times a term/word came up in each act. Let’s click on new worksheet to get started. Let’s rename this one to “Pie”.

    <img src='{{ '/assets/images/ReReTableauWorkshop3-3.jpg' | relative_url }}' alt='Spreadsheet frequencies by Term, Count and Act are outlined with a red box. New Worksheet icon at the bottom left are outlined with a red box' title='' width='1241' height='735' />
4. Let’s first make a simple pie chart to show how many words are in each Act of the play, to see which Act is the longest and shortest and how they contribute to the whole.
5. Before we begin building our visualization, let’s make sure our variables are correct. If we look at what the variable types Tableau’s has identified in our dataset, you’ll notice that it thinks Act is a numeric variable in the Measures section, when really it is categorical in this case. So let’s change it to move it to our Dimensions section. Drag the Act variable into the Dimensions section.  
    
    <img src='{{ '/assets/images/ReReTableauWorkshop3-5.jpg' | relative_url }}' alt='Term, Measure Names and Act are outlined with red boxes under the Tables menu on the left' title='' width='510' height='418' />
6. Using Show Me, hold down the Control Key and click on Act and Count (hold down the Command Key if on Mac), and then expand the Show Me tab. I see that pie chart is one of the recommendations. Let’s pick it.

    <img src='{{ '/assets/images/ReTableauWorkshop3-6.jpg' | relative_url }}' alt='Act and Count are highlighted and outlined with red boxes under the Tables menu on the left. Show Me and the pie chart icon at the top right are outlined with red boxes' title='' width='1600' height='752' />
7. It is very small, so let’s make it larger by selecting Entire View from the ribbon drop\-down.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop3-7.jpg' | relative_url }}' alt='Entire View from the ribbon drop-down is outlined with a red box' title='' width='972' height='785' />
8. Next, let’s label it. Drag Act on to Label, and then Count on to Label. Then click on Label, and click on the ... icon next to the Text field to edit the label.

    <img src='{{ '/assets/images/ReTableauWorkshop3-8.1.jpg' | relative_url }}' alt='Act is outlined with a red box under the Tables menu on the left. The Label icon is outlined with a red box under the Marks card. The ... button is outlined with a red box next to the Text field' title='' width='689' height='577' />

    Add the word “Act” to just before the \<Act\> number to clarify the label, and then click on OK. Then click away to close the window  
    
    <img src='{{ '/assets/images/ReTableauWorkshop3-8.2.jpg' | relative_url }}' alt='Text box and OK button are outlined with red boxes' title='' width='540' height='330' />
9. Currently it is showing the frequency count as a raw number, but we could show a percentage of the total instead, which is more common for pie charts. Right click on the SUM (Count) Label Pill (the last one listed on the Marks card). Select Quick Table Calculation and then Percent of Total.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-9.jpg' | relative_url }}' alt='Sum(Count) under the Marks card is outlined with a red box. Quick Table Calculation and Percent of Total are outlined with red boxes' title='' width='684' height='736' />
10. We could also format the percentages to round to whole numbers. Right click on the SUM (Count) Label Pill again, and this time select Format.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-10.1.jpg' | relative_url }}' alt='Sum(Count) under the Marks card and Format... are outlined with red boxes' title='' width='970' height='760' />  
    From the Format window that appears on the left, in the Pane tab, under the Default section, from the drop\-down for Numbers, select Percentage and then change the number of Decimal places to zero. Then click away to close the window.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-10.2.jpg' | relative_url }}' alt='Pane, Numbers, Percentage, and Decimal places are outlined with red boxes' title='' width='725' height='660' />
11. We can see the number of words used is quite evenly distributed throughout the acts, but Act 3 uses the most and Act 5 uses the least.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-11.jpg' | relative_url }}' alt='' title='A pie chart is displayed' width='1059' height='761' />

 

## Creating Scatter Plots

1. Sometimes you have to pull data from multiple sources instead of having it all in one file. Let’s add a couple more datasets, but this time we’re going to match them up or join them together to create one large dataset to work from.
2. Go to the top Data Menu and select New Data Source.  

    <img src='{{ '/assets/images/ReTableauWorkshop4-2.1.jpg' | relative_url }}' alt='Data and New Data Source are outlined with red boxes at the top left' title='' width='700' height='255' />

    Select Microsoft Excel.  

    <img src='{{ '/assets/images/ReReTableauWorkshop4-2.2NEWNEW.jpg' | relative_url }}' alt='Microsoft Excel is outlined with a red box' title='' width='1007' height='890' />

    Choose AuthorDataCitationsGrants.xls.  
    
    <img src='{{ '/assets/images/ReReTableauWorkshop4-2.3New.jpg' | relative_url }}' alt='AuthorDataCitationsGrants.xls is outlined with a red box' title='' width='1048' height='614' />  
        
    This is the dataset containing names of authors, their countries and institutions, research interests, how many citations they’ve received over a few years, and how much grant money they’ve received over a few years.
    <img src='{{ '/assets/images/ReReReTableauWorkshop4-2.4New.jpg' | relative_url }}' alt='AuthorDataMain table information is outlined with a red box' title='' width='1316' height='879' />
3. Now click on “Add” next to Connections on the top left to add a second dataset, select Microsoft Excel.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-3.jpg' | relative_url }}' alt='Add and Microsoft Excel are outlined with red boxes' title='' width='1055' height='658' />  
    
    Then pick the AuthorDataExperience.xls file. This dataset has just author names along with how many years of experience they have as a researcher.  

    <img src='{{ '/assets/images/ReReTableauWorkshop4-3.2.jpg' | relative_url }}' alt='AuthorDataExperience.xls outlined with a red box' title='' width='1055' height='643' />
4. To relate or connect the two datasets, drag AuthorDataExperience under Sheets over to the section where it says, “Need more data?” (if you don't see AuthorDataExperience under Sheets, make sure that AuthorDataExperience is selected under Connections).  

    <img src='{{ '/assets/images/ReTableauWorkshop4-4.1.jpg' | relative_url }}' alt='AuthorDataExperience under Sheets and Need more Data? Are outlined with red boxes' title='' width='1120' height='613' />  

    The bottom window shows us that the data has been related together based on a common column, Author. Now the years of experience data will also be associated with the appropriate authors additional data found in the first table. Tableau performs relates and joins on the fly, as needed. If these terms are new to you, see these articles on [relationships](https://help.tableau.com/v2020.2/pro/desktop/en-us/datasource_relationships_learnmorepage.htm) and [joins](https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins) in the slides.

    <img src='{{ '/assets/images/ReReTableauWorkshop4-4.2New.jpg' | relative_url }}' alt='AuthorDataMain, Operator and AuthorDataExperience outlined with a red box' title='' width='826' height='358' />
5. Then we can click on the New Worksheet icon at the bottom. Let’s rename this one to “Scatter Plot”.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-5A.jpg' | relative_url }}' alt='The New Worksheet icon at the bottom left is outlined with a red box' title='' width='325' height='196' />  
​​​​​
6. Scatter Plots are great to use to identify if there is any relationship between numeric variables. Let’s see if there is a relationship between grants and years of experience.
7. Again, let’s create this scatterplot using the Show Me feature. This time, hold down the Control Key and click on Grants and Years of Experience (hold down the Command Key if on Mac), and then expand the Show Me tab. I see that Scatter Plot is one of the recommendations. Let’s pick it.

    <img src='{{ '/assets/images/ReTableauWorkshop4-7.jpg' | relative_url }}' alt='Years of Experience and Grants outlined with red boxes under the Tables menu on the left. Scatter Plot icon outlined with a red box under the Show Me menu at the top right' title='' width='1593' height='771' />
8. Doesn’t look like much yet, but let’s make some adjustments. First, instead of summing these variables, let’s take the averages. So right click on the Grants Pill next to Rows, select Measures (Sum) and then change it to Average. Do the same for the Years of Experience Pill next to Columns.  

    <img src='{{ '/assets/images/ReTableauWorkshop4-8.jpg' | relative_url }}' alt='SUM(Years of Experience), SUM(Grants) with Measure (Sum) and Average outlined with red boxes' title='' width='811' height='609' />
9. Our next problem is that it is plotting just one x/y pair – the averages of the whole dataset. We need to plot the points either for each Author, Country, or Institution. Let’s do it by Author. This is where that Details box comes up. If you drag Author over it, it explodes out the aggregation to plot it by Author.  

    <img src='{{ '/assets/images/ReTableauWorkshop4-9.jpg' | relative_url }}' alt='Author under the Tables menu on the left and Detail under the Marks label are outlined with red boxes' title='' width='762' height='635' />

    When you hover over a point, you can see the details.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-9.2.jpg' | relative_url }}' alt='Scatter Plot shown' title='' width='808' height='657' />
10. You may notice there is now also another box on the Marks card called Shape. If you want to add another categorical variable to your Scatter Plot, you could do so by using different shapes to represent different categories. Drag Institution on to the Shape box. Now you should see that there is a legend on the right, using different shapes for different institutions.
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-10.jpg' | relative_url }}' alt='Institution under the Tables menu, Shape under the Marks label is outlined with red boxes. Institution legend shown and outlined with a red box at the top right' title='' width='1583' height='676' />
11. If you want to add trend lines in Tableau, right\-click in the centre and select Trend Lines \-\> Show Trend Lines.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-11.1.jpg' | relative_url }}' alt='Trend Lines and Show Trend Lines are outlined with red boxes' title='' width='990' height='663' />  

    Hovering over the lines also gives you statistical information, such as P\-values.  

    <img src='{{ '/assets/images/ReTableauWorkshop4-11.2.jpg' | relative_url }}' alt='Scatter Plot shown' title='' width='797' height='534' />
12. Finally, one interesting feature of Tableau is to create not just one visualization, but a series of them, using the Pages shelf. Drag Year on to the Pages shelf.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-12.1.jpg' | relative_url }}' alt='Year under the Tables menu and Pages in the centre area are outlined with red boxes' title='' width='378' height='463' />

    Now you should see some controls on the right. The user can scroll through three different Scatter Plots, one for each year, or they can click on the Play button to have it animate through the years.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-12.2.jpg' | relative_url }}' alt='Year scatter plots control bar outlined with a red box' title='' width='1210' height='724' />

 

## Creating Dashboards

1. Now so far we’ve been creating visualizations within worksheets. But you can also create Dashboards that combine a number of visualizations together to present a more complex story than a single visualization can show. So for example, let us click on the Create New Dashboard icon at the bottom, next to the New Worksheet icon.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-1.jpg' | relative_url }}' alt='Create New Dashboard icon at the bottom, next to the New Worksheet icon is outlined with a red box' title='' width='571' height='274' />
2. You then can drag and drop various sheets to layout a dashboard. You can see it really helps to label your sheets. You can also drag other Objects (bottom left), such as text or images to create your dashboard. So let’s create a Dashboard showing Sales and Profit by Sub\-Category and being able to filter by State/Province.  

    <img src='{{ '/assets/images/ReReReReTableauWorkshop5-2.jpg' | relative_url }}' alt='Sheets options menu shown' title='' width='209' height='350' />
3. Before we start building our dashboard, I just want to adjust the Sales Bar sheet slightly. Go to it by clicking on its tab at the bottom.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-3.1.jpg' | relative_url }}' alt='Sales Bar at the bottom is outlined with a red box' title='' width='580' height='255' />

    Right click on the State/Province filter, and select Edit Filter...  

    <img src='{{ '/assets/images/ReTableauWorkshop5-3.2.jpg' | relative_url }}' alt='State/Province under Filters and Edit Filter... are both highlighted and outlined with red boxes' title='' width='926' height='598' />
4. Select All and click on OK.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-4.1.jpg' | relative_url }}' alt='All and OK buttons are outlined with red boxes' title='' width='453' height='566' />

    Then right click the State/Province filter again, but this time select Show Filter.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-4.2.jpg' | relative_url }}' alt='State/Province under Filters and Show Filter... are both highlighted and outlined with red boxes' title='' width='599' height='532' />

    Now you can see the filters show up on the right. Hover over the legend until you see a small arrow. Click on it to get the drop\-down menu, then select Single Value (dropdown). Now we have a State/Province filter that the reader can use to filter the graph. We’re going to take this filter and use it in our Dashboard to apply to all the graphs we add into the Dashboard.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-4.3.jpg' | relative_url }}' alt='State/Province drop-down arrow at the top right and the Single Value (dropdown) are outlined with red boxes' title='' width='1206' height='647' />
5. So let’s go back to our Dashboard by clicking on the Dashboard 1 tab at the bottom.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-5.jpg' | relative_url }}' alt='Dashboard 1 tab at the bottom is outlined with a red box' title='' width='756' height='367' />
6. First, let’s drag the Sales Bar sheet into the Dashboard.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-6.1.jpg' | relative_url }}' alt='Sales Bar under Sheets and Drop sheets here are outlined with red boxes' title='' width='1148' height='715' />

    Then drag the Line sheet underneath and select a few categories of interest.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-6.2.jpg' | relative_url }}' alt='Line under Sheets and the bottom half of the categories are outlined with red boxes' title='' width='1170' height='706' />

    Your Dashboard should now look like this.  
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-6.3.jpg' | relative_url }}' alt='Sales by Sub-Category for All dashboard is shown' title='' width='980' height='737' />
7. Our Dashboard seems a bit squished, so to improve how it displays, under Size on the left, change Fixed size to Automatic.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-7A.jpg' | relative_url }}' alt='Size on the left, drop-down icon and Automatic are outlined with red boxes' title='' width='735' height='558' />
8. To make the filter for the Sales sheet apply to both, right click on the title of the filter, State/Province, select Apply to Worksheets, and then pick Selected Worksheets...  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-8.1.jpg' | relative_url }}' alt='State/Province, Apply to Worksheets, and Selected Worksheets are outlined with red boxes' title='' width='718' height='383' />

    Click on Select all on dashboard in the pop\-up window, and then click on OK. Now you’ll see that when you select one State/Province, both graphs refer to that State/Province. End up picking all States/Provinces.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-8.2.jpg' | relative_url }}' alt='Select all on dashboard and OK button are outlined with red boxes' title='' width='699' height='402' />
9. Let’s add a title to our Dashboard. Drag Text from under Objects to the top of the Dashboard. As you drag, make sure the grey rectangle is narrow, spanning the top of the whole Dashboard.  
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-9.1.jpg' | relative_url }}' alt='Grey rectangle at the top of the dashboard and Text under the Objects menu at the bottom left are outlined with red boxes' title='' width='1588' height='848' />

    Make the title “Sales and Profit by Sub\-Category”, set the font size to 20 and make it bold. Resize the height of the title to finish it off.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-9.2.jpg' | relative_url }}' alt='B icon to bolden text and OK button are outlined with red boxes' title='' width='544' height='324' />

    Your Dashboard should now look like this.
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-9.3.jpg' | relative_url }}' alt='The updated dashboard is shown' title='' width='1383' height='833' />
10. Finally, let’s add a Dashboard Action, where if you click on a Sub\-Category in one of the graphs, it’ll highlight it in both to help the reader link the data together visually. From the Dashboard menu at the top, select Actions...  
    
    <img src='{{ '/assets/images/TableauWorkshop5.10-1.jpg' | relative_url }}' alt='Dashboard at the top left and Actions... are outlined with red boxes' title='' width='502' height='362' />

    Click on Add Action and select Highlight... From this window, you could customize the settings if you wish to specify which sheets would be affected, and when the action will occur, for example.  
    
    <img src='{{ '/assets/images/TableauWorkshop5.10-2.jpg' | relative_url }}' alt='Add Action and Highlight are outlined with red boxes' title='' width='494' height='355' />

    Let’s keep the defaults and click on OK. Then click OK again.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-10.3.jpg' | relative_url }}' alt='The OK button at the bottom right is outlined with a red box' title='' width='501' height='676' />

    Now if you select a Sub\-Category in one graph, such as the Arts Sub\-Category in the Bar Graph, it should highlight it in the second graph (highlighting the line). Click it again to deselect it.
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-10.4.jpg' | relative_url }}' alt='The dashboard is shown with the Art Sub-Category highlighted with a red box' title='' width='1384' height='833' />
11. Once you’ve created some visualizations and Dashboards, your last steps are to save and publish them. If you’re working on some visualizations, like we have here, you can save work\-in\-progress as a Tableau Workbook file. Go to the File menu and click on Save. Give it a name and select where you want to save the file. (Note: If you do this, it doesn’t save the underlying data, so you have keep the data file(s) and workbook together). Or you can select Export Packaged Workbook… (also from the File menu). Then you could share that file with others who have Tableau (and this time it includes the data). In both cases, you can then come back to revisit your work later by reopening it in Tableau Desktop.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-11.jpg' | relative_url }}' alt='Save and Export Packaged Workbook... from the File menu at the top left are outlined with red boxes' title='' width='324' height='608' />
12. If you want to export one of your worksheets to an image you can use in a report or article, you can do so from the Worksheet menu. There are options to either Export it as an image or Copy it and paste it into a document or image editing software to work with it further. You can do the same thing for your whole Dashboard or Story from the Dashboard or Story menu respectively.
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-12.jpg' | relative_url }}' alt='Copy and Export are outlined with red boxes from the Worksheet menu at the top left' title='' width='952' height='657' />
13. As our Dashboard and visualizations can also be interactive, there may be times when you want to publish them to the web so that your users can view them. Your free option is to create a [Tableau Public](https://public.tableau.com/app/discover) account and publish it there using that option in the Server menu (but note it is public; however, you can adjust the settings, if you don’t want readers to download the underlying data and/or workbook). There are also pay options ([Tableau Cloud](https://www.tableau.com/products/cloud-bi) and [Tableau Server](https://www.tableau.com/products/server)), if you want to be able to limit permissions on who can view your visualizations or to publish to your own server; use the Publish Workbook option from the Server menu to access these options.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-13.jpg' | relative_url }}' alt='Server at the top is outlined with a red box' title='' width='715' height='349' />
14. If you also go to [Tableau Public Viz of the Day](https://public.tableau.com/app/discover/viz-of-the-day), you’ll see Tableau visualizations to provide inspiration. If there’s something you’re interested in, you can click on the Download icon (a small box with an arrow pointing down) at the bottom to see if you can download the workbook. You can also click on the Share icon (three staggered dots connected by lines) to share the visualization.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14B.jpg' | relative_url }}' alt='The Download icon and the Share icon are outlined with red boxes at the bottom right' title='' width='1537' height='1180' />

    When downloading the visualization, you can click Data to download the workbook used for this visualization (if the Data button is not greyed out). You can then open the workbook to see how the author created this visualization.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14.2.jpg' | relative_url }}' alt='Data and Tableau Workbook buttons are outlined with red boxes in the download menu' title='' width='256' height='298' />

    When sharing the visualization, you can access its Embed Code. If you want to embed your own visualizations into your own website, you have to first upload them to Tableau Public, then click on the share icon to get the embed code to add to your website’s HTML code.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14.3.jpg' | relative_url }}' alt='Embed Code is outlined with a red box' title='' width='262' height='205' />

And that’s it!

Technique: [Data Visualization](/technique/data-visualization) \| Tools: [Tableau](/tools/tableau)

**Date Created:** 2022\-08\-31 **Updated:** 2023\-01\-30
