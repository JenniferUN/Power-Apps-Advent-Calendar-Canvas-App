# Power-Apps-Advent-Calendar-Canvas-App
Beautiful Advent Calendar built using native Power Apps canvas controls

1️⃣ Import the Canvas App
1.	Download the **AdventCalender.zip** and the **Advent.xlsx** spreadsheet.
2.	Go to https://make.powerapps.com/ and click on **Apps** then click on **Import app > From package (.zip).**
 ![Import app](docs/images/Step1.png)
3.	On the Import package screen change the setup to **Create as new** and click **Import**. 
  ![Import app screen](docs/images/Step2.png)
4.	Wait a couple of minutes for the app to import into your environment.
5.	Click Edit the app.
![Import app](docs/images/Step3.png)
6.  You’ll notice that there are a number of errors in the app. We’ll fix that in the next steps when we create our data source in SharePoint.
![App with errors](docs/images/Step4.png)

2️⃣ Prepare the SharePoint List

1.	Create a new list in a SharePoint site of your choice. 
 ![Create a list in SharePoint](docs/images/Step2_1.png)
2.	Select Import From **Excel**
  ![Create a list in SharePoint](docs/images/Step2_2.png)
3.	Set the data types as follow:
•	Day: Number
•	Date: Date and time
•	Title: Title
•	Message: Multiple lines of text
•	Image: Do not import
•	Action: Choice
•	Action Description: Single line of text
•	Link: Single line of text
•	Attachment: Do not import
•	Email Subject: Single line of text
•	Email Message: Multiple lines of text
4.	Click Next and name the list **AdventCalendar* then click **Create.**
  ![Create a list in SharePoint](docs/images/Step2_3.png)
5.	Once the list is created, you’ll need to update some settings for the Date, Message, Action and Email Message columns.
6.	Go to List Settings
   ![Create a list in SharePoint](docs/images/Step2_4.png)
7.	On the List Settings screen, scroll down and select the **Date** column.
  ![Create a list in SharePoint](docs/images/Step2_5.png)
8.	Change the ‘Date and Time format’ to **Date Only** and click **OK.**
9.	Now select the **Message* column from the list. In the ‘Specify the type of text to allow:’ select **Enhanced rich text (Rich text with pictures, tables, and hyperlinks)** and click **OK.**
  ![Create a list in SharePoint](docs/images/Step2_6.png)

10.	Repeat step 9 for the **Email Message** column as we need to ensure that both of these columns can render Rich Text and HTML.
11.	Finally, select the Action column from the list.
12.	Add the following choice options:
•	Link
•	Email
•	Download
13.	Ensure that the **Default value** field is left blank.
14.	Click **OK**
  ![Create a list in SharePoint](docs/images/Step2_7.png)
SharePoint setup is now complete. In the next steps, we will fix the data connections in the app.



