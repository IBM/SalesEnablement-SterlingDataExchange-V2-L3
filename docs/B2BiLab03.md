Lab3 simulates an EDIFACT EDI interchange being received by B2B Integrator and processed into an application file.

The import does not have to be part of the demonstration.   The business process, maps,  envelopes etc. are imported into B2B integrator.  

## Open the B2Bi dashboard and import the lab03 definition

1. In the B2B Integrator web console, click **Import/Export** under the **Resource Manager** under **Deployment** in the left-hand panel.

![](_attachments/B2BiLab03-01-Go-To-Import.png)

1. Click **GO** 
   
![](_attachments/B2BiLab03-02-Select-Go-To-Import.png)

??? question "BP quiz question"
    Several BP quiz questions will come from this area **B2Bi Import**. When taking the BP quiz make sure tyou have noted the number of maps imported.

1. Click **Choose File** in the **Import Resources** page.

![](_attachments/B2BiLab03-03-Click-Choose-File.png)

4. Select the **Lab03_Import.xml**  This may look different depending upon what platform you are importing the xml from.

![](_attachments/B2BiLab03-04-Select-File-From-Desktop.png)

5. Enter **password** into the Passphrase dialog box and click **Next**

![](_attachments/B2BiLab03-05-Enter-Import-password.png)

1. No changes to Resource Tags so click **Next** 

![](_attachments/B2BiLab03-06-Skip-Create-Resource-Tag.png)

5. Leave the default to allow updates if objects exist in the system.   Click **Next**



![](_attachments/B2BiLab03-06-Accept-Update-Objects-Default.png)

!!! hint
    Note sure what to hint about here....if anything.....

1. Use the **double down arrow** to select all of the TP (Trading Partner) Envelopes

![](_attachments/B2BiLab03-07-Import-TP-Envelopes.png)


In the latest {{offering.name}} release, new password policies have been set that require users to change their password the first time they authenticate. 

7. The trading partner envelopes are shown as all selected. Click **Next** 

![](_attachments/B2BiLab03-08-TP-Envelopes-Selected.png)


1. Use the **double down arrow** to select all of the Maps.  Then click **Next**

![](_attachments/B2BiLab03-09-Import-Maps.png)


1. Use the **double down arrow** to select all of the Users.  Then click **Next**

![](_attachments/B2BiLab03-10-Import-Users.png)


1. Use the **double down arrow** to select all of the Permissions.  Then click **Next**

![](_attachments/B2BiLab03-11-Import-Permissions.png)


1. Use the **double down arrow** to select all of the Mailbox Virtual Root.  Then click **Next**

![](_attachments/B2BiLab03-12-Import-Mailbox-Virtual-Root.png)

1. Leave the default of **Select All**  Then click **Next**

![](_attachments/B2BiLab03-13-Import-Mailbox-Metadata.png)

1. Use the **double down arrow** to select all of the Mailbox Routing Rules.  
   
![](_attachments/B2BiLab03-14-Import-Mailbox-Routing-Rule.png

1.    All of the artifacts selected for import are shown.   If any are missing, hit the **Back** button and make the additional selections.    Otherwise, click **Finish**

![](_attachments/B2BiLab03-15-Confirm-Import.png)


1.    Click **Return** 

![](_attachments/B2BiLab02-12-Return-From-Imports.png)

!!! important "Important"

    That is the end of the setup necessary for the lab.   In a customer demo situation, that should usually get setup ahead of time so that only the following steps are needed to show the demo scenario itself.


## Execute the lab03 demo ---  NEED TO UPDATE WITH JAMES

13.  Click **Business Processes** and then **Manager**. In the Search box enter **lab02** to search for the process name. 

![](_attachments/B2BiLab02-19-Enter-BP-Selection.png)


??? question "BP quiz question"
    Not sure what question best here ir even if the popp up is functioning.

14. Click on the **Execution Manager** 

![](_attachments/B2BiLab02-20-Select-BP-to-Run.png)


15.  Click **Execute** to run the business process. 

![](_attachments/B2BiLab02-21-Execute-Business-Process.png)

16.  In the **Local Desktop filename** Select **Choose File**  
   
![](_attachments/B2BiLab02-22-Select-Input-File.png)


17.  On the desktop itself choose the input file **outb810.txt** from the file system.  
 
!!! Note "Note"

    Generally, documents sent by the B2B Integrator host company to trading partners are considered "outbound" and ANSI X12 invoices are "810"s, hence the outb810 name.  This contents and formatting of this file is critical for the proper functioning of the business process.  The file format is typical of many flat file formatted application files.  The file is processed by two different maps in the Business Process.   The first finds the partner name off an internal supplier number in the application file.   The second translates the contents of the file into into an ANSI X12 EDI format.  is the end of the setup necessary for the lab.   In a customer demo situation, that should usually get setup ahead of time so that only the following steps are needed to show the demo scenario itself.

![](_attachments/B2BiLab02-23-Select-Input-File-on-PC.png)

18.   Once the file is shown as selected next to **Choose File** click **GO!**

![](_attachments/B2BiLab02-24-Press-Go-to-Execute-BP.png)

19.  Wait until the Business Process completes and all of the Status are shown as **Success** Click **Close** in the upper right of the screen.

![](_attachments/B2BiLab02-25-View-Completed-Processes.png)

## View the Business Process Results

Now that the Business Process has run, the user can view detail of the process.  

20.   Click **Current Processes** under **Monitor** which is under **Business Process**

![](_attachments/B2BiLab02-26-Select-Current-Processes.png)

21. Click the **ID** next to the **Lab02_Process_Positional** step
    
![](_attachments/B2BiLab02-27-Select-Start-of-Process.png)

22.   Inside the  **Lab02_Process_Positional** click on **info** in the first line under the **Document** column

![](_attachments/B2BiLab02-28-Select-Input-File-in-Process.png)

23.  The Input application file is shown.  This is the format coming out of an Accounts Receivable module most likely in an ERP system.  Close out of this screen.

![](_attachments/B2BiLab02-29-View-Input-File-In-Process.png)

24.  Click on the top process in the **Id** Column.

![](_attachments/B2BiLab02-30-Select-End-of-Process.png)

25.  View the final output document by clicking on **info** in the last row under the **Document** column. 

![](_attachments/B2BiLab02-31-Select-Final-Output.png)


26.   The output ANSI X12 document is shown.   

![](_attachments/B2BiLab02-32-View-Final-Output-as-EDI.png)

??? question "BP quiz question"
    There is a quiz question somewhere around here....


This concludes lab02. 

