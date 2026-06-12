---
title: Creating Dashboards
parent: Tableau Workshop Demonstration Tutorial
layout: default
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2022-08-31
nav_order: 6
---

## Creating Dashboards

1. Now so far we’ve been creating visualizations within worksheets. But you can also create Dashboards that combine a number of visualizations together to present a more complex story than a single visualization can show. So for example, let us click on the Create New Dashboard icon at the bottom, next to the New Worksheet icon.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-1.jpg' | relative_url }}' alt='Create New Dashboard icon at the bottom, next to the New Worksheet icon is outlined with a red box' title='' width='571' height='274' />
2. You then can drag and drop various sheets to layout a dashboard. You can see it really helps to label your sheets. You can also drag other Objects (bottom left), such as text or images to create your dashboard. So let’s create a Dashboard showing Sales and Profit by Sub-Category and being able to filter by State/Province.  

    <img src='{{ '/assets/images/ReReReReTableauWorkshop5-2.png' | relative_url }}' alt='Sheets options menu shown' title='' width='209' height='350' />
3. Before we start building our dashboard, I just want to adjust the Sales Bar sheet slightly. Go to it by clicking on its tab at the bottom.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-3.1.jpg' | relative_url }}' alt='Sales Bar at the bottom is outlined with a red box' title='' width='580' height='255' />

    Right click on the State filter, and select Edit Filter...  

    <img src='{{ '/assets/images/ReTableauWorkshop5-3.2.jpg' | relative_url }}' alt='State under Filters and Edit Filter... are both highlighted and outlined with red boxes' title='' width='926' height='598' />
4. Select All and click on OK.  

    <img src='{{ '/assets/images/ReTableauWorkshop5-4.1.jpg' | relative_url }}' alt='All and OK buttons are outlined with red boxes' title='' width='453' height='566' />

    Then right click the State filter again, but this time select Show Filter.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-4.2.jpg' | relative_url }}' alt='State/Province under Filters and Show Filter... are both highlighted and outlined with red boxes' title='' width='599' height='532' />

    Now you can see the filters show up on the right. Hover over the top of the list until you see a small arrow. Click on it to get the drop-down menu, then select Single Value (dropdown). Now we have a State filter that the reader can use to filter the graph. We’re going to take this filter and use it in our Dashboard to apply to all the graphs we add into the Dashboard.  
    
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
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-7A.png' | relative_url }}' alt='Size on the left, drop-down icon and Automatic are outlined with red boxes' title='' width='451' height='839' />
8. To make the filter for the Sales sheet apply to both, right click on the title of the filter, State, select Apply to Worksheets, and then pick Selected Worksheets...  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-8.1.png' | relative_url }}' alt='State, Apply to Worksheets, and Selected Worksheets are outlined with red boxes' title='' width='718' height='383' />

    Click on Select all on dashboard in the pop-up window, and then click on OK. Now you’ll see that when you select one State, both graphs refer to that State. End up picking all States.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-8.2.jpg' | relative_url }}' alt='Select all on dashboard and OK button are outlined with red boxes' title='' width='699' height='402' />
9. Let’s add a title to our Dashboard. Drag Text from under Objects to the top of the Dashboard. As you drag, make sure the grey rectangle spans the top of the whole Dashboard.  
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-9.1.png' | relative_url }}' alt='Grey rectangle at the top of the dashboard and Text under the Objects menu at the bottom left are outlined with red boxes' title='' width='1588' height='848' />

    Make the title “Sales and Profit by Sub-Category”, set the font size to 20 and make it bold. You can also centre it, if you'd like. Resize the height of the title box to finish it off.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-9.2.jpg' | relative_url }}' alt='B icon to bolden text and OK button are outlined with red boxes' title='' width='544' height='324' />

    Your Dashboard should now look like this.
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-9.3.jpg' | relative_url }}' alt='The updated dashboard is shown' title='' width='1383' height='833' />
10. Finally, let’s add a Dashboard Action, where if you click on a Sub-Category in one of the graphs, it’ll highlight it in both to help the reader link the data together visually. From the Dashboard menu at the top, select Actions...  
    
    <img src='{{ '/assets/images/TableauWorkshop5.10-1.png' | relative_url }}' alt='Dashboard at the top left and Actions... are outlined with red boxes' title='' width='502' height='362' />

    Click on Add Action and select Highlight... From this window, you could customize the settings if you wish to specify which sheets would be affected, and when the action will occur, for example.  
    
    <img src='{{ '/assets/images/TableauWorkshop5.10-2.png' | relative_url }}' alt='Add Action and Highlight are outlined with red boxes' title='' width='494' height='355' />

    Let’s keep the defaults and click on OK. Then click OK again.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-10.3.jpg' | relative_url }}' alt='The OK button at the bottom right is outlined with a red box' title='' width='501' height='676' />

    Now if you select a Sub-Category in one graph, such as the Art Sub-Category in the Bar Graph, it should highlight it in the second graph (highlighting the line). Click it again to deselect it.
    
    <img src='{{ '/assets/images/ReReReTableauWorkshop5-10.4.jpg' | relative_url }}' alt='The dashboard is shown with the Art Sub-Category highlighted with a red box' title='' width='1384' height='833' />
11. Once you’ve created some visualizations and Dashboards, your last steps are to save and publish them. If you’re working on some visualizations, like we have here, you can save work-in-progress as a Tableau Workbook file. Go to the File menu and click on Save. Give it a name and select where you want to save the file. (Note: If you do this, it doesn’t save the underlying data, so you have keep the data file(s) and workbook together). Or you can select Export Packaged Workbook… (also from the File menu). Then you could share that file with others who have Tableau (and this time it includes the data). In both cases, you can then come back to revisit your work later by reopening it in Tableau.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-11.jpg' | relative_url }}' alt='Save and Export Packaged Workbook... from the File menu at the top left are outlined with red boxes' title='' width='324' height='608' />
12. If you want to export one of your worksheets to an image you can use in a report or article, you can do so from the Worksheet menu. In Tableau Desktop (only), there are options to either Export it as an image or Copy it and paste it into a document or image editing software to work with it further. You can do the same thing for your whole Dashboard from the Dashboard menu.
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-12.jpg' | relative_url }}' alt='Copy and Export are outlined with red boxes from the Worksheet menu at the top left' title='' width='952' height='657' />
13. As our Dashboard and visualizations can also be interactive, there may be times when you want to publish them to the web so that your users can view them. Your free option is to create a [Tableau Public](https://public.tableau.com/app/discover) account and publish/save it there using that option in the Server menu for Tableau Desktop (or from the File menu for Tableau Public), but note it is public; however, you can adjust the settings, if you don’t want readers to download the underlying data and/or workbook. There are also pay options ([Tableau Cloud](https://www.tableau.com/products/cloud-bi) and [Tableau Server](https://www.tableau.com/products/server)), if you want to be able to limit permissions on who can view your visualizations or to publish to your own server; use the Publish Workbook option from the Server menu to access these options (Tableau Desktop only).  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-13.jpg' | relative_url }}' alt='Server at the top is outlined with a red box' title='' width='715' height='349' />
14. If you also go to [Tableau Public Viz of the Day](https://public.tableau.com/app/discover/viz-of-the-day), you’ll see Tableau visualizations to provide inspiration. If there’s something you’re interested in, you can click on the Download icon (a small box with an arrow pointing down) at the bottom to see if you can download the workbook. You can also click on the Share icon (three staggered dots connected by lines) to share the visualization.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14B.png' | relative_url }}' alt='The Download icon and the Share icon are outlined with red boxes at the bottom right' title='' width='1537' height='1180' />

    When downloading the visualization, you can sometimes download the workbook used for this visualization (if it is not greyed out). You can then open the workbook to see how the author created this visualization. You can also use this menu as a workaround for Tableau Public users in order to download a static image of your visualization.
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14.2.png' | relative_url }}' alt='The download options are outlined with a red box' title='' width='256' height='298' />

    When sharing the visualization, you can access its Embed Code. If you want to embed your own visualizations into your own website, you have to first upload them to Tableau Public, then click on the share icon to get the embed code to add to your website’s HTML code.  
    
    <img src='{{ '/assets/images/ReTableauWorkshop5-14.3.png' | relative_url }}' alt='Embed Code is outlined with a red box' title='' width='262' height='205' />

And that’s it!

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Tableau](https://mdlutoronto.github.io/tutorials-search/?tool=Tableau)