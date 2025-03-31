# maxent_ex
This is a tutorial for using Maxent with basic features. I will walk you through a basic run and a little help with interpretting the output. First of all, download this repository somewhere on your computer and make sure it is unzipped.

## Install 
Go to [https://biodiversityinformatics.amnh.org/open_source/maxent/], go to the Download section, and fill in the information to download. A zip file will appear wherever your browser is set to put downloads. Please unzip the file, enter the resultant folder, and double-click the Java JAR file.

Note that you will need a working Java environment. If it turns out you don't have this (e.g., some recent Macs), you will need to plan some lead time as this takes a while to download. 

On a Mac environment, you may have security features preventing you from opening the JAR file. Just right-click > open with > JavaLauncher and the program will be given permission. Depending on where you downloaded this repository, you may also be prompted for further access permissions.

## Run 
When you have the JAR file open, you will have a GUI environment to set. In the top left dialog, select one CSV file from the `occurrences` folder of this repository (using your local download). Then in the top right dialog, select the folder labeled `pacific_northwest_layers`. (Do not enter the folder or try to click anything in it.)

At this point, Maxent will populate a number of default settings. It is good practice to familiarize yourself with these. We will modify a few. Check the box that says "Create response curves." Also click the box that says "Do jackknife to measure variable importance." Set the "Projection layers directory/file" dialog to the `projection_layers` folder in this repository. 

Now click "Settings"; you will be in the "Basic" tab at the top. Click "Random seed." Set "Random test percentage" to 25. Set "Replicates" to 10. Change "Replicated run type" to "Bootstrap." Go to the "Advanced" tab of settings at the top. Uncheck "extrapolate" (think about why). Go to the "Experimental" tab at the top. Check "Use samples with some missing data." If you understand the processor your computer has, you can set the "Threads" option accordingly; if you are unfamiliar with multithreading, "1" is fine. Exit the dialog. Set the output directory to something appropriate. You can use the empty folders I have prepared for you: `output` > `Genus_species_model` etc.
