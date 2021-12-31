# PowerBI-GoogleTimeline
Source pbix file and instructions for using Power BI to interrogate and export personal Google timeline data. May be useful in assisting COVID contract tracers

------------

This report initially loads with cached sample data.  To visualise and extract your own timeline data follow the steps below.

<b>Step 1: Download your Google Timeline data</b>
<ul>
<li>Go to Google Takeout - https://takeout.google.com/ </li>
<li>Deselect everything apart from Location History </li>
<li>Scroll to bottom and click Next Step </li>
<li>Select preferred compression and file split size (defaults should be fine) </li>
<li>Click on Create Export. You will be warned that this export could take days but have found when only exporting Location Data it takes only a few minutes. The report will appear in the same screen, you will receive an email when complete. </li>
<li> Click on Download link provided (Authenticate if required). A compressed file will be saved to the downloads folder for your browser. </li>
</ul>

<b> Step 2: Extract Relevant Files </b>

<ul>
<li> This Power BI report is set to look for data in a folder called  C:\Semantic Location History.  Create this folder (or modify the code in power query to look in your alternative location) </li>
<li>Open the downloaded compressed file and copy everything under \Takeout\Location History\Semantic Location History into this folder. The folder should now contain a folder for each year with each year containing json files for each month. </li>
  </ul>

<b> Step 3: Analyse in Power BI </b>
<ul>
<li>In Power BI click on Home > Refresh to load your data. </li>
<li>Select the desired time window using the slicer on the top left. </li>
<li>Location tags (such as Home and Work) will show in the filter where used. These can be included / excluded from the data set to declutter the list.  </li>
<li>The filtered location table can be exported to CSV by hovering over the table clicking on the ellipsis that appear and selecting Export Data. </li>
  </ul>



