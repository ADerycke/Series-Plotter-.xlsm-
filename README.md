![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/b424b0f9-6329-48d9-bb85-59c1af6edd63)

# Series-Plotter : General introduction

This file ***Series plotter(version).xlsm*** is simply made to accelerate significantly Excel chart production, and add other kind of chart not natively handle by Excel (e.g., ternary diagram, stacked "temporal" chart...).
The file also has tools for geosciences like :
  - allowing to add grid for binary and ternary diagram, with a list of already implemented geochemical grids (cf. grid file).
  - allowing to automatically normalise geochemical data, with a list of already implemented geochemical normalisation (cf. normalisation file).

It's never perfect so maybe you gonna encounter some troubles and errors, so don't hesitate to report me any problem.
There is no restriction to use and distribute the "Series Plotter" files, as long as you refer this GitHub. 

*Excel version :*
  - should work on any version earlier than Excel 2016
  - never tested on version older than Excel 2016
  - some utilities/tools may not work on the restrained version of Excel (as students version or application)

*Systems :*
  - Windows 10 (32bit) : not tested but should work
  - Windows 10 (64bit) : tested and work
  - Windows 11 (64bit) : not tested but should work
  - MacOS (Monterey) : tested and work for most of the main functionnalities
  
For the MacOS user, several development facilities are not included in Mac Excel, so i'm working on correcting bug and make work all the functionnalities... but it take time.
List of know problems : save as .pdf (but save as .svg...), export in a .ppt (not natively possible by now)....

**Conceptor : Alexis Derycke** 
  - [Reseach Gate](https://www.researchgate.net/profile/Alexis-Derycke)

# Summary :
**- [How to use the file](#part_1)**

**- [How to set-up the layout (color, shape,...)](#part_2)**

**- [Graphic type](#part_3)** : *XY , XYZ (Z as color), ternary diagram, vertical stacked XY, spider diagram, normalisation, grids,...*

**- [How to select the X-Y-Z axes in the "Graphics list" sheet](#part_4)**


# How to use the file <a id="part_1"></a> 
You just have to download the file, opening it and allow the macro execution. To help you to understand the file, there is some tips (like the real excel) that pop if you let your mouse above most of the button :

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/1529f0e0-fc43-4baa-90cd-df656b282ed9)

You can also find several videos (~2min) in the helping folder that gonna introduce you to the file and show you quickly how to use it. Associate data examples are in the folder to easily test the series plotter and reproduce what its show in videos.

If you want to simply play with Series Plotter, you can click on **"Data template"** in the ***HELP*** group and it gonna automatically add a dataset to play with.

**Step by Step simple use :**
  - step 1 : open the file and **allow macro execution**
  - step 2 : add some data. You can do it as any other excel sheets, or click on **"Data template"**. The data structuration is quite simple : first row = hearder, second row = unit, thrid row = empty.
  - step 3 : retriver your data header. To do so, click on the **"Get column"** button
  - step 4 : chose the data to plot. To do so, go on the **"Graphic list"** sheet and select the corresponding position in the grid
  - step 5 : chose the type of plot. To do so, clik on dropdown **"Select the graphic(s) type"** in the ribbon and select the wanted plot (e.g. "XY - classic")
  - step 6 : chose the header with sample ID. To do so, clik on the **left** dropdown of **"sample determination"** in the ribbon and select the appropriate header (e.g. "Name") 
  - step 7 : generate the graphic(s). To do so, click on **"Plot Graphic"** button
  
For more options, let your mouse on any button and a screen tips gonna appear, or read the following documentations

https://github.com/ADerycke/Series-Plotter/assets/130437433/d620555c-989c-427b-a564-139f6c200737

# How to set-up the layout (color, shape,...) : <a id="part_2"></a> 

All graphs/plots are full Excel graphs/plots (event more complex one as stacked or ternary plot), so you can edit/copy/use them like any other Excel graphs/plots.

Additionally, to this manual editing, you can modify several parameters for all graphs/plots automatically using the ribbon or the "Layout" sheets.

## Ribbon options :

**OPTION (Series)**

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/7e28bd85-5ad5-4c12-b5ea-2dc64b13573b)

You can find all the options to change and retriver the series layout. "Set series layout" will open a small windows to edit series layouts of all graph at the same time. "Get series color" will retriver the series colors form a graph for the next plotting. "Get graph layout" allow you to completely custom your graph and use this layout for latter plot. 

**OPTION (Chart)**

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/e1a645b5-b9b3-40aa-b588-8d93d606c719)

You can find all the options related to the chart/graph

## Sheets "Layout" options :

It's not mandatory to use this sheets, it's only if you want to setup and re-use custom serie layout.

You can right click on cells of the "Color" column and a colors selection window gonna appear, after the selection the cell gonna take the color you select.

You can copy and past the color obtains to all cells, it gonna work. If you remove the value inside the cell, then the color goes back to "nul", meaning automatic to excel.

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/277658b7-6458-4106-8b56-4ff51611f52a)


If you select multiple cells, then it gonna automatically generate a color gradient : 

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/a5df3ba4-0fd5-4a5e-a9ee-46f76744accd)


# Graphic type : <a id="part_3"></a> 

## graphic XY :

![graph XY](https://user-images.githubusercontent.com/130437433/233654680-7dec2505-8e34-4ba6-90ac-d4c969450cd1.png)

**note :** for binary diagram, multiple automatic grid are already ready to add to graph
![image](https://user-images.githubusercontent.com/130437433/233656030-1236a5e2-c85f-40e5-a94c-f834610e12a8.png)

![graph XY - grid](https://github.com/ADerycke/Series-Plotter/assets/130437433/9b0c2ee8-5b1b-4162-a395-3155466ece9f)

## graphic XYZ (Z as color) :

![Zcolor - 1](https://github.com/ADerycke/Series-Plotter/assets/130437433/e610d7d9-df17-44d7-8f63-23b37830a7f5)

**note :** min and max value are determined automatically from the dataset. You can select a third color and indicate its value. You can also select an automatic round of the min and max value.
![Zcolor](https://github.com/ADerycke/Series-Plotter/assets/130437433/f04832a0-ecdb-4d51-8944-dd2c03fe736f)

## graphic XYZ (ternary diagram) :

![graph XYZ](https://user-images.githubusercontent.com/130437433/233654854-ad3199e7-f194-4f03-9329-8e0e1341f9b2.png)
![graph XYZ (bis)](https://user-images.githubusercontent.com/130437433/233799016-01b8f8f8-f5e9-4137-879a-6b409bcc31da.png)

**note :** for ternary diagram, multiple automatic grid are already ready to add to graph

![image](https://user-images.githubusercontent.com/130437433/233655226-8d13ca9e-ea7e-4495-881e-ff361bf8c55b.png)


## graphic XY - stacked :

![graph XY - stacked ](https://user-images.githubusercontent.com/130437433/233655423-5dc175fc-9fe8-4177-9faa-4711021abeee.png)

## graphic Y (spectra/spider diagram) :

![graph Y](https://user-images.githubusercontent.com/130437433/233655533-995ee4f8-3b7d-4268-9f38-8be0b044d1d1.png)

**note :** for spider diagram, an automatic normalisation is possible (msg pop-up at the selection).
This normalisation gonna be applied/remove to your data in fonction of what you want.
The available normalisation can be found and selected on the "Normalisation" sheet that apprear after it selection.
![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/f1bc2a27-678e-45de-a50b-678474d599d0)

## Normal law and KDE calculation :

![graph Normal law](https://github.com/ADerycke/Series-Plotter/assets/130437433/97ad0c89-154d-4c71-9103-68ade5a1e215)

## weigth mean plot and calculation :

![graph-Ages  Ma](https://github.com/ADerycke/Series-Plotter/assets/130437433/35dc744b-c9ff-48b1-bfc7-cf359496fc8a)

## X - Histogram (automatic generation) :

![X - Histogram](https://github.com/ADerycke/Series-Plotter/assets/130437433/e660c782-9aeb-4ce7-b2be-4eb6e6be83f6)

**note :** when you select this, you enter the wanted range (here 6 to 18) and the wanted interval (here 1) and excel gonna automatically calculate the distribution in your dataset

## Fit of multiple gaussian to a KDE distribution :

![graph preak determination](https://github.com/ADerycke/Series-Plotter/assets/130437433/60c02689-7a26-4d8c-9543-2034f2f3c29d)

# How to select the X-Y-Z axes in the "Graphics list" : <a id="part_4"></a> 

## graphic XY :
Just enter X and Y axes ...

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/886f5d18-8c44-4e45-ae9d-afa8800e0d94)

## graphic XYZ (Z as color) : 
the Z axe is read in the area as the X axe

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/b77def31-8547-4183-8472-4f9240847829)

## graphic XYZ (ternary diagram) :
the 3 pole of the ternary diagram is read only on the Y axe (add a fourth one to get a double ternary diagram)

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/8aea9da8-be10-4dc4-aa75-7b892bd0f987)

## graphic XY - stacked :
you can use same or different X axes for the time

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/e87bc40f-29a3-4be0-b348-8c5842243cb1)

## graphic Y (spectra/spider diagram) :
use only the Y axe to enter the data to plot (data in the same row will be plotted together)

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/a319a9e3-47b7-438c-997b-8b320f0488f7)

## Normal law and KDE (basic distribution) :
no need of the "Graphics list", just select the data you want to analyse and clik on the proper button (column 1 : data, optinal : column two : error)

## weigth mean plot and calculation :
no need of the "Graphics list", just select two column (column 1 : data, column two : error) you want to analyse and clik on the proper button

## X - Histogram (automatic generation) :
use only the X axe to determine the data to plot

![image](https://github.com/ADerycke/Series-Plotter/assets/130437433/f21c0779-f18b-4f8e-89cf-2969ae9236b9)

## Fit of multiple gaussian to a KDE distribution :
no need of the "Graphics list", just select the data you want to analyse and clik on the proper button (column 1 : data, optinal : column two : error)
