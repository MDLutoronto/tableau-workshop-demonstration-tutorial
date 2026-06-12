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

1. We are going to start with a dataset from Tableau. If you are using Tableau Desktop, the dataset is built in. Under Saved Data Sources, select Sample - Superstore. 

    <img src='{{ '/assets/images/TableauWorkshop1.1.jpg' | relative_url }}' alt='The Tableau home screen is shown with Sample – Superstore outlined with a red box at the bottom left' title='' width='1642' height='971' />

    OR If you are using Tableau Public, you will need to first download the [Superstore Sales dataset from Tableau](https://public.tableau.com/app/sample-data/sample_-_superstore.xls). Then in Tableau, we need to load the data. Click on Microsoft Excel under Connect To a File. Select the superstore file. Drag the Orders sheet into the blank space to the right of it to select that sheet from the Excel workbook. Finally, click on Sheet 1 at the bottom.

    <img src='{{ '/assets/images/Tableau_Demo_BarGraph_001b.png' | relative_url }}' alt='The Tableau home screen is shown with Microsoft Excel outlined with a red box at the bottom left' title='' width='1642' height='971' /> 
    <img src='{{ '/assets/images/Tableau_Demo_BarGraph_001c.png' | relative_url }}' alt='The superstore Excel file and the Open button outlined with red boxes' title='' width='1642' height='971' /> 
    <img src='{{ '/assets/images/Tableau_Demo_BarGraph_001d.png' | relative_url }}' alt='The Tableau data loading screen is shown with the Orders sheet outlined with a red box and an arrow indicating to the right to illustrate dragging it to the right' title='' width='1642' height='971' /> 
    <img src='{{ '/assets/images/Tableau_Demo_BarGraph_001b.png' | relative_url }}' alt='The Tableau data loading screen is shown with Sheet 1 outlined with a red box at the bottom left' title='' width='1642' height='971' /> 


2. Let’s look around first before we dive in. On the left you can see Tables listed. Within a Table, the variables are listed, but divided by a thin grey line. Tableau categorizes variables as either Dimensions (above the line) or Measures (below the line). Dimensions are roughly qualitative data and Measures are roughly quantitative data.

    <img src='{{ '/assets/images/ReTableauWorkshop1-2.jpg' | relative_url }}' alt='Under the Tables menu on the left, Dimensions and Measures variables are outlined with a red box.' title='' width='1220' height='883' />
3. The centre area is where you’ll be dragging and dropping your variables on to different areas, such as Rows and Columns, or to vary Marks like Colour or Size by your variable, or filtering by a variable. Those areas that say Filters or Pages are called Shelves.

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.2.jpg' | relative_url }}' alt='The Pages and Filters boxes are outlined with a red box.' title='' width='896' height='576' />
4. The Marks area have what are called cards, and when the variables are showing up in those areas, they are called pills, as they are shaped like a pill. 

    <img src='{{ '/assets/images/ReReTableauWorkshop1-3.3.jpg' | relative_url }}' alt='The Marks area is outlined with a red box underneath the Pages and Filters boxes' title='' width='943' height='728' />  
    
    We’ll take a look at all these options as we go through the demo. One of the useful features of Tableau, to take a look at when you’re new to the tool and/or data visualization, is the Show Me feature. If you hold down Control and click on a couple of variables (hold down Command if on Mac), and then expand the Show Me tab, you’ll see that Tableau is giving you suggestions for what type of visualization to use by outlining the recommended visual.  

    <img src='{{ '/assets/images/TableauWorkshop1.2-2.jpg' | relative_url }}' alt='Order Date and Order ID are highlighted in blue and outlined with a red box under the Tables menu on the left. The Show Me menu is outlined with a red box on the top right' title='' width='1657' height='970' />
5. Okay, we’ve loaded in some data about a US fictional superstore, so let’s start by creating some visualizations that are used to make comparisons. Let’s start by making a simple bar graph. To keep track of all the visualizations we’re going to create, let’s rename our sheets as we go. Right-click on Sheet 1 at the bottom, select Rename, and give it the name “Sales Bar” and press Enter.

    <img src='{{ '/assets/images/ReTableauWorkshop1-3.jpg' | relative_url }}' alt='Sheet 1 at the bottom left and Rename from the pop-up menu are outlined with a red box' title='' width='' height='636' />
6. We’re going to create a horizontal bar graph to compare the amount of sales for different subcategories of products, with Sub-Category along the y-axis and Sales along the x-axis. Bar graphs are great for comparing categories. So drag the Sales variable (in the Measures section) next to Columns and Sub-Category (in the Dimensions section) next to Rows.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-6.jpg' | relative_url }}' alt='A horizontal bar graph called Sales Bar is shown with Sub-Category along the y-axis and Sales along the x-axis. The Sales variable shown as SUM(Sales) is in the Columns and Sib-Category is in the Rows at the top' title='' width='1370' height='737' />
7. You can see that when we dragged Sales, Tableau automatically summarized it by adding up all the Sales values for each Sub-Category. Right now it is showing data combined for all of the States (this is a US example), but let’s say we just want it to show one of them. We can filter by State by dragging the State variable (in the Dimensions section) over to the Filters shelf and selecting one State from the list.

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
12. You normally drag a variable on to the Detail section to clarify to what level of detail are marks on the page displayed at. We’ll look an example of this later.
13. Finally, the Tooltip section allows you to customize the text and format in the pop-up that shows up when you hover or click on a particular bar. For example, let’s add the broader Category that the product falls under in the Tooltip. To do this, drag the Category variable (in the Dimensions section) to the Tooltip box.

    <img src='{{ '/assets/images/TableauWorkshop1.11-1.jpg' | relative_url }}' alt='Category under the Tables menu on the left is outlined with a red box. Tooltip under the Marks card is outlined with a red box' title='' width='1174' height='685' />  
        Then click on Tooltip. In the edit box, you’ll see that Category has been added underneath Sub-Category to the Tooltip. However, if you want to change the order, perhaps to have the broader category go first, you can click on Tooltip and edit the box. Let’s switch the order and click on OK.

    <img src='{{ '/assets/images/ReTableauWorkshop1-11.2.jpg' | relative_url }}' alt='OK is outlined with a red box in the Edit Tooltip menu' title='' width='548' height='409' />
14. As you can see there are options to customize a lot of parts of the visualization. You can also customize the axes. For example, right-click on your x-axis title, select Edit Axis...

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.1.jpg' | relative_url }}' alt='Edit Axis... is outlined with a red box near the x-axis of the horizontal bar graph' title='' width='1172' height='644' />

    Let's edit the x-axis Title next to Custom to say 'Sales in US Dollars'. Once we are done there's no OK button to click, just close the window, as the changes have already been applied.

    <img src='{{ '/assets/images/ReTableauWorkshop1-12.2.png' | relative_url }}' alt='The Sales in US Dollars Custom Axis Title at the bottom is outlined with a red box in the Edit Axis [Sales] pop-up window' title='' width='449' height='644' />
15. Right now the bars are sorted in alphabetical order by Sub-Category, but if you hover over the x-axis label, Sales in US Dollars, a small sort icon appears. Click on it to sort your bars by Sales instead. Every time you click the icon, it cycles through different sort orders. Let’s have it sort descending with the Sub-Category with the largest sales at the top. You can now easily see the top and bottom sub-categories in terms of sales.

    <img src='{{ '/assets/images/ReTableauWorkshop1-13.jpg' | relative_url }}' alt='The Sort Icon at the centre bottom of the horizontal bar graph is outlined with a red box' title='' width='1164' height='605' />
16. If we wanted to, we could also spread this visualization out a bit, so it isn’t squished up at the top. From the top ribbon where it says Standard, use the drop-down to select Entire View.  

    <img src='{{ '/assets/images/ReTableauWorkshop1-14.jpg' | relative_url }}' alt='The drop-down menu from the top ribbon is outlined with a red box with Entire View highlighted' title='' width='1373' height='868' />
17. Finally, we can give our visualization a more meaningful title by double clicking where it says “Sales Bar” at the top. You’ll see the default title is the sheet name, but we can change that. Let’s put “Sales by Sub-Category for “ then instead of typing in “California”, we can make the title dynamic by click on Insert and selecting State. Then if we change the filter, the title will automatically change.   

    <img src='{{ '/assets/images/ReTableauWorkshop1-15.png' | relative_url }}' alt='The Insert drop-down menu at the top right and State/Province near the bottom of the drop-down options are outlined with a red box' title='' width='658' height='495' />

Now we’re done our first visualization!

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)