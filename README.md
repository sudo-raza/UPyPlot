# UPyPlot
### Plot Unity script variables in realtime using MatPlotLib


![alt tag](https://raw.githubusercontent.com/guiglass/UPyPlot/master/SceneLayout.png)

**What is it:**

The intention of this example was to build an easy to use plotting tool for visualizing the values generated by AI controllers and to see how their PID loops were affecting vehicles causing them to overshooting/undershooting or act unexpectedly.

_This tool was designed to help diagnose multiple variables across multiple scripts as quickly and painlessly as possible._

**Prerequisites:**

* This was built using Unity 2017, but earlier versions sould support the feature set.
* Python 2.7 with MatPlotLib and NumPy installed.

**How to use:**

It's simple to add any private or public variable to the plot. This is done by adding a **[UPyPlot.UPyPlotController.UPyProbe]** custom attribute to the variable decloration, after which you should see that variable in the plot.

---
![alt tag](https://raw.githubusercontent.com/guiglass/UPyPlot/master/ExampleAttributes.png)
---


**_Integrating with your own project:_**

* Copy the UPyPlot folder and all of it's contents from this example's assets folder to your projects assets folder.
* Place the UPyPlotController prefab into your scene.
* Ensure the output filename matches what is set in PlotViewer.py (default is plot.txt).
* Add the [UPyPlot.UPyPlotController.UPyProbe] attribute to any variable you want shown in the plot.
* Run the PlotViewer.py Python file and start your scene (in any order). 
* Enjoy.


**Configuration:**
At present the tool offers some configurability such as:
![alt tag](https://raw.githubusercontent.com/guiglass/UPyPlot/master/InspectorOptions.png)

* Precision - _Number of decimal places for each value in the plot data file._
* Interval - _Rate in seconds which to update plot data file with new values._
* Max Samples - _Maximum lines/history that the plot file should contain._


**Advanced Viewer (UPyPlotAdvancedViewer.py):**

I have also added a second Python script (similar to the basic viewer) that has an additional button for changing the plot style from a single plot to individual plots:

_Note that the individual mode appears to update at a slightly reduced rate when compared to the combined mode. I may address this in a future update._
![alt tag](https://raw.githubusercontent.com/guiglass/UPyPlot/master/Advanced.png)

---

Please feel free to use this example in any way you see fit (without restriction of any kind) as well as redistribute, modify and share it with all of your friends and co-workers.

Legal notice:
By downloading or using any resource from this example you agree that I (the author) am not liable for any losses or damages due to the use of any part(s) of the content in this example. It is distributed as is and without any warranty or guarantees. 

*Project by: Grant Olsen (jython.scripts@gmail.com)
Creation year: 2017*





