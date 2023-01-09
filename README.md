# Workflow-Action

# Description
In this project I'll demonstrate how to create a workflow action in splunk. Workflow action allows a person to access web resources from using the "Get" , "post" and "search" method.The "Get" method is used to create a html link and use that link to search field values. The "Post" method is used to put an HTTP post request for a specific url, lastly the "search" method allows you too use field values to perform a secondary search for an event.


<h1>Step 1</h1>
Start on the splunk home screen and hover over the settings, click on the settings and find "Knowledge". This is where all of the knowledge objects reside , clicking "fields" there will be a numerous of fields extraction you can choose from to modify your data. But today we are specifically working with the "workflow action", before we create our workflow action we want to look at the field we will be using in our underline search in the search and reporting app.

This is the basic search i'm using , I want to make a workflow action using the "get" method for the "clientip" field. My goal for this field is to retrieve information about the clientip from a website called "whois.domaintools.com".
<br>
<img src="https://imgur.com/8RBXtFu.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>

<br>
<img src="https://imgur.com/gK6QF02.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>


<h2>Step 2</h2>
This is the view of configuring the workflow action, its very simple method. You can practice on your own using different fields from your indexes.

Once you save your configuration , head back to the search and reporting app to confirm the workflow action has been successful configured.

<br>
<img src="https://imgur.com/XBq6pDy.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>

<br>
<img src="https://imgur.com/qCSBPYJ.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>

<h3>Step 3</h3>
Confirm the workflow action is searchable and retrieves you to the website you listed in the configurations. You run the search which should have the respected field, for example my search is "index=sam sourcetype=* " Once the events populate i'll click on one of the events then click "Event Action" and my workflow is displaying. 

<br>
<img src="https://imgur.com/SieRyRU.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>

When you click on your workflow action it should open a new tab displaying the information of that specific IP address for that event.

<br>
<img src="https://imgur.com/Bnu8sDi.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</br>
