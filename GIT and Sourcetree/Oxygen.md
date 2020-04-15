# Oxygen Install and Transformation Scenario

## Install Oxygen XML Editor

1. Download the software at http://www.oxygenxml.com/xml_editor/software_archive_editor.html  

2. Choose version 15.2.  

3. Copy and paste information below into the license window:  

   Registration_Name=Gregory Neville  

   Company=University of North Carolina at Chapel Hill  

   Category=Academic-Site  

   Component=XML-Editor, XSLT-Debugger, Saxon-SA Version=15  

   Number_of_Licenses=1 Date=06-13-2013  

   Maintenance=374 SGN=MCwCFFnvMwFb46l7evGVjmLvrQHbLdc+AhR4SOcVT5QvkKKRj1EdgHZDzj/+mA\=\=      
   
## Set up transformation scenario

(Occasionally, you may have to recreate a new transformation scenario. Sometimes they just go away.) 

1. Open an EAD XML file in Oxygen. 

2. Click on the top horizontal menu's icon of a wrench with a red arrow 

3. In the pop-up box, select "New." 

4. Name your scenario something simple like "transformation_2018" 

_In the XSLT tab:_

5. XML URL should be "${currentFileURL}" (which it will be by default). 

6. XLS URL should point to our stylesheet: http://cdn.lib.unc.edu/faids/ead.xsl 

7. Select the transformer. Saxon EE 9.5.1.3. 

![Edit scenario screenshot 1](https://user-images.githubusercontent.com/58087302/79362917-2f21b380-7f15-11ea-8399-1f86a66559ea.png "Edit scenario window screenshot 1")

We don't use the FO Processor tab

_In the Output tab:_

8. In the Output File menu, the "Save as" box should be selected, and the value should be: "${cfn}.html" 

9. If you would like for the resulting HTML file to automatically open in your Internet browser for preview, or in Oxygen for you to inspect, check the boxes for these options. 

10. Click "OK." You will be returned to the opening menu, but now you will see your new scenario appearing in the list of available transformation scenarios. 

> Note: If you forgot to name your scenario, it will automatically be named after the EAD XML file that you had opened when you began creating the scenario. To rename it, select it in the list and click "EDIT." Then change the name across the very top of the menu. Click "OK" to save your new scenario and return to Oxygen. 

![Edit scenario screenshot 2](https://user-images.githubusercontent.com/58087302/79363266-afe0af80-7f15-11ea-9754-3ce394c71b3c.png "Edit scenario window screenshot 2")


