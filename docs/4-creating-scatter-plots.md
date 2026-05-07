---
title: Creating Scatter Plots
parent: Tableau Workshop Demonstration Tutorial
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2022-08-31
nav_order: 4
---

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
11. If you want to add trend lines in Tableau, right-click in the centre and select Trend Lines -> Show Trend Lines.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-11.1.jpg' | relative_url }}' alt='Trend Lines and Show Trend Lines are outlined with red boxes' title='' width='990' height='663' />  

    Hovering over the lines also gives you statistical information, such as P-values.  

    <img src='{{ '/assets/images/ReTableauWorkshop4-11.2.jpg' | relative_url }}' alt='Scatter Plot shown' title='' width='797' height='534' />
12. Finally, one interesting feature of Tableau is to create not just one visualization, but a series of them, using the Pages shelf. Drag Year on to the Pages shelf.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-12.1.jpg' | relative_url }}' alt='Year under the Tables menu and Pages in the centre area are outlined with red boxes' title='' width='378' height='463' />

    Now you should see some controls on the right. The user can scroll through three different Scatter Plots, one for each year, or they can click on the Play button to have it animate through the years.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop4-12.2.jpg' | relative_url }}' alt='Year scatter plots control bar outlined with a red box' title='' width='1210' height='724' />

Technique: [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| Tools: [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)