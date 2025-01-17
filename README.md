# The FreeCAD Airplane Design Workbench
[![Total alerts](https://img.shields.io/lgtm/alerts/g/FredsFactory/FreeCAD_AirPlaneDesign.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/FredsFactory/FreeCAD_AirPlaneDesign/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/FredsFactory/FreeCAD_AirPlaneDesign.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/FredsFactory/FreeCAD_AirPlaneDesign/context:python)  
A FreeCAD workbench dedicated to Airplane Design  

**Warning:** This is highly experimental code. Testers are welcome.

![AirPlaneDesign-UI-screen](resources/WingResult.png)

![WingProfile-screenshot](resources/AirplaneDesign001.png)

## Release Notes
**v0.4**: 
New Object : Plane, Wing and WingPanel. 
New Wing generator.
Naca Rib generator.

**v0.3**: NACA Rib generator  
**v0.2**: New release with parametric objects based on a dedicated UI  
**v0.1**: Initial release based on sheet  deprecated!

**v0.001**: 11 July 2018: Initial version

## Prerequisites
* FreeCAD >= v0.18
install "Plot"  & "Curved shapes" WorkBench.

## Installation
Use the FreeCAD [Addon Manager](https://github.com/FreeCAD/FreeCAD-addons#installing) from the tools menu to install AirPlaneDesign Workbench.
You will also require Plot and CurvedShapes addons (both also available in the Addon Manager)

## Quickstart
There are various examples available. Under Windows these are in: C:\Users\USERNAME\AppData\Roaming\FreeCAD\Mod\AirPlaneDesign\examples

To create your own from scratch:
After installation a new Airplane Design menu and toolbar will be available
You must first "Create a plane" (you can give it dimensions but it won't be visible)
Ensure the plane is selected in the navigation window and select "Create/Add a wing to plane"
Ensure the wing is selected in the navigation window and select "Wing Wizard"
Click "Fill in Sheet With Example" to create the demo wing

## Usage

The menu contains with the following functions:  
1. Create a rib : you can import DAT file or generate NACA Profile.
1.1 Import a DAT File
Simply copy the DAT File in the folder

![DAT folder](resources/Ribsfolder.png)
1.2 Create a Rib based on a DAT file
In the menu AiplaneDesign select create a RIB, the dialog below appears, click on the tab "Import DAT File".

![DAT folder](resources/RIBSGUI1.png)

Select in the tree the dat file you want to use and define the chord of the rib and clic OK. That's all.
You can change directly in the GUI of the object the Dat File, the chord (in mm). 

1.3 Use the NACA Generator
You can generate Naca profil 4 or 5 digits. In the menu AiplaneDesign select create a RIB, the dialog below appears, click on the tab "NACA Generator". Simply fill the NACA Number, the number of points you want to generate and the chord in mm. A preview is automatically generated. 

![RibGUI](resources/RibGUI.png)


2.Create a wing


![WingGUI](resources/WingGUI.png)

The result

![WingGUI](resources/WingResult.png)



Ability to choose the:  
* Profiles you want to import in the UI (.dat format)  
 **Note:** 2 profiles are installed with the workbench ([eppler 205](wingribprofil/e205.dat) and [eppler 207](wingribprofil/e207.dat)). If you'd like to use different profile(s), simply include said .dat file(s) in to the [`wingribprofil`](wingribprofil/) directory.

## Roadmap

V0.4 :
- [X] Add NACA profil generator
- [X] Add Preview profil and sheet
- [X] Implement rib thickness and NACA finite TE by adrianinsaval
- [X] Improve wing design UI
- [X] Wing object
- [X] Wing Panel Object
- [ ] Improve RIB file selection 
- [ ] Import profil from UIUC Airfoil Database
- [ ] Add ability to translate workbench
- [ ] Tutorials

V0.5 : Some ideas....
- [ ] Generate Rib from Wing
- [ ] Xfoil integration
- [ ] Increase the width of wizard dialog box so the rotation columns are visible
- [ ] Add option to Automatically generate a mirror wing for the other side
- [ ] Wing wizard remembers settings from previous wing
- [ ] Copy and paste the wing wizard table (eg to and from a spreadsheet)
- [ ] More "complete plane" example files (eg like the GordLoft_4 example)
- [ ] Fuselage design module
- [ ] Add an "open folder" or "install profile" button in the rib design dialog to make it easier to find/add extras
- [ ] ----------
- [ ] ----------

## Feedback
Feedback can be provided via the [discussion thread in english](https://forum.freecadweb.org/viewtopic.php?f=8&t=42208) or [discussion thread in french](https://forum.freecadweb.org/viewtopic.php?f=12&t=40376) on the FreeCAD forums  
Some dicussions here : https://forum.freecadweb.org/viewtopic.php?f=3&t=41159&p=356564#p356564

## License
LGPLv2.1  
See [LICENSE](LICENSE) file


