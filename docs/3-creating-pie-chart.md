---
title: Creating Pie Charts
parent: Tableau Workshop Demonstration Tutorial
layout: default
nav_order: 3
---

## Creating Pie Charts

1. Let’s try loading our own data – this time some qualitative humanities data. Tableau is not meant to work directly with text data files, but you can use other better-suited textual analysis tools to create datasets that you can then visualize in Tableau. What I did was take the freely available text for Shakespeare’s play Romeo and Juliet. I ran it through a free online tool called [Voyant Tools](https://voyant-tools.org/) and it generated a word frequency table that we are now going to use as our dataset. If you want to learn more about textual analysis and visualization tools, such as Voyant, you can take a look at the [Tools & Tutorials page](https://mdl.library.utoronto.ca/dataviz/tools-tutorials) in the [data viz guide](https://mdl.library.utoronto.ca/dataviz/getting-started).  

    <img src='{{ '/assets/images/ReTableauWorkshop3-1.jpg' | relative_url }}' alt='Voyant home screen is shown' title='' width='1004' height='521' />
2. Let’s load this word frequency data into Tableau. Again, go to Data->New Data Source.  

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
7. It is very small, so let’s make it larger by selecting Entire View from the ribbon drop-down.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop3-7.jpg' | relative_url }}' alt='Entire View from the ribbon drop-down is outlined with a red box' title='' width='972' height='785' />
8. Next, let’s label it. Drag Act on to Label, and then Count on to Label. Then click on Label, and click on the ... icon next to the Text field to edit the label.

    <img src='{{ '/assets/images/ReTableauWorkshop3-8.1.jpg' | relative_url }}' alt='Act is outlined with a red box under the Tables menu on the left. The Label icon is outlined with a red box under the Marks card. The ... button is outlined with a red box next to the Text field' title='' width='689' height='577' />

    Add the word “Act” to just before the <**Act**> number to clarify the label, and then click on OK. Then click away to close the window  
    
    <img src='{{ '/assets/images/ReTableauWorkshop3-8.2.jpg' | relative_url }}' alt='Text box and OK button are outlined with red boxes' title='' width='540' height='330' />
9. Currently it is showing the frequency count as a raw number, but we could show a percentage of the total instead, which is more common for pie charts. Right click on the SUM (Count) Label Pill (the last one listed on the Marks card). Select Quick Table Calculation and then Percent of Total.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-9.jpg' | relative_url }}' alt='Sum(Count) under the Marks card is outlined with a red box. Quick Table Calculation and Percent of Total are outlined with red boxes' title='' width='684' height='736' />
10. We could also format the percentages to round to whole numbers. Right click on the SUM (Count) Label Pill again, and this time select Format.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-10.1.jpg' | relative_url }}' alt='Sum(Count) under the Marks card and Format... are outlined with red boxes' title='' width='970' height='760' />  
    From the Format window that appears on the left, in the Pane tab, under the Default section, from the drop-down for Numbers, select Percentage and then change the number of Decimal places to zero. Then click away to close the window.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-10.2.jpg' | relative_url }}' alt='Pane, Numbers, Percentage, and Decimal places are outlined with red boxes' title='' width='725' height='660' />
11. We can see the number of words used is quite evenly distributed throughout the acts, but Act 3 uses the most and Act 5 uses the least.  

    <img src='{{ '/assets/images/ReTableauWorkshop3-11.jpg' | relative_url }}' alt='' title='A pie chart is displayed' width='1059' height='761' />