# Tranformation Scenario

Occasionally, you may have to create a new transformation scenario. Sometimes they just go away. Open an EAD XML file in Oxygen. 

- Click on the top horizontal menu's icon of a wrench with a red arrow

- In the pop-up box, select "New."

- Name your scenario something simple like "transformation_2017"

In the XSLT tab:

- XML URL should be "${currentFileURL}" (which it will be by default). 

- XLS URL should point to our stylesheet: http://cdn.lib.unc.edu/faids/ead.xsl 

- Select the transformer. Saxon EE 9.5.1.3. 

![Edit scenario window](https://user-images.githubusercontent.com/58087302/78826539-a902eb80-79af-11ea-9a4b-68fba90374ee.png "Window 1")

We don't use the FO Processor tab

In the Output tab:

- In the Output File menu, the "Save as" box should be selected, and the value should be: "${cfn}.html" 

- If you would like for the resulting HTML file to automatically open in your Internet browser for preview, or in Oxygen for you to inspect, check the boxes for these options. 

- Click "OK." You will be returned to the opening menu, but now you will see your new scenario appearing in the list of available transformation scenarios. 

> Note: If you forgot to name your scenario, it will automatically be named after the EAD XML file that you had opened when you began creating the scenario. To rename it, select it in the list and click "EDIT." Then change the name across the very top of the menu. Click "OK" to save your new scenario and return to Oxygen. 

![Transformation window](https://user-images.githubusercontent.com/58087302/78826705-f717ef00-79af-11ea-8eac-b89053d1a68d.png "Window 2")
