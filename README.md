#Generation of boxes suitable for laser cut machine

##Presentation

To house the various design made with our Fablab, laser-cut boxes are frequently used. I decided to create an Inkscape extension to make various kind of boxes, all in the same extension. The created boxes are more decorative, than simple rectangular boxes, at least I hope so!
I like rounded corners, so the created boxes can have rounded corners (1 to 4 rounded corners), with different radiuses.
It is also possible to have "slots" inside the box, we can set the number of columns and rows.
An example of what is possible to do:

<center>![Genbox_1](https://user-images.githubusercontent.com/35993911/69336078-5920c380-0c5e-11ea-80a9-4cab35be853f.png)</center>
 
##Hardware 

Nothing ... Except wood to get to get real! <br> 
Use rather thin wood (3 or 5mm max). I personally used MDF or plywood.
The MDF supports the Flex, the plywood a little less well, but it's still possible, be careful though!
You could also use other material suitable for laser cut machine, such as PMMA.


## Boxes type 

Here are some pictures of boxes made with this extension. The list is not exhaustive, the program is generic and you can combine various possibilities.

### Rounded corners

Each corner can be rounded with a different radius. A radius  at 0 gives a straight corner. Attention, it is not necessarily possible to go below 10mm, the wood is not so flexible! <br>
The 4 corners can be rounded, here with the same radius of curvature. Here I chose, a simple cover <br>

<center>![Boite_Arrondie_01](https://user-images.githubusercontent.com/35993911/69336379-abfa7b00-0c5e-11ea-9606-e3e4086e7419.JPG)</center><br>

You can also have this style of shape with the opposite corners rounded, always with a simple lid, note in this case the presence of slots in the box: <br>

<center>![SimpleTop_02](https://user-images.githubusercontent.com/35993911/69336476-e2d09100-0c5e-11ea-808a-8c8685298e87.JPG)</center><br>
<center>Box with simple lid</center><br>

### Lid style
The extension offers 7 types of lid
1. Without lid: no top for the box, no notches on the top
2. Closed box: the top fits with notches like the other faces. Solid, but not necessarily easy to disassemble!
3. Simple top: the lid is obtained by gluing the piece without a notch that encloses the box and the inside cut with notches. This allows the lid to hold while easily removing. This is shown in the image above.
4. Sliding lid: The lid slides on the top of the box. Notches on the sides allow to hold the lid and handle it easily. See example below. Attention in this case, the finished box is a little higher (2 times the thickness of the wood) to accommodate the slide system.
5. Lid with wooden hinge: Here the box is surmounted by small "ears" playing the role of hinge. Everything is wood, with MDF it works very well. With plywood, it is also possible, but it slides a little less well and makes a little noise during openings and closures. See also the example below. The lid can rotate up to 180 °, it rests in case on the back side.
6. Metal Hinge Cover: The hinges consist of small pieces of wood rotating around a metal shaft. I realize this axis from a nail (2.3 or 2.4mm diameter, sorry not in inch !) cut to the right dimension with a cutting pliers. The lid can also rotate 180 °. See picture below.
7. Chest style: This lid uses the same type of hinge as the previous one, but the top is curved, as in a chest! This type of lid is incompatible with rounded corners. <br>

<center>![Sliding_01](https://user-images.githubusercontent.com/35993911/69336551-07c50400-0c5f-11ea-8036-f1e671141f3a.JPG)]</center><br>
<center>Sliding top</center><br>

<center>![IWood_01](https://user-images.githubusercontent.com/35993911/69336588-1f9c8800-0c5f-11ea-9f2a-caf73890aaf0.JPG)</center><br>
<center>Wood hinge</center><br>

<center>![Charniere_Metal_02](https://user-images.githubusercontent.com/35993911/69336628-3cd15680-0c5f-11ea-8421-768f504c6fbc.JPG)</center><br>
<center>Steel hinge</center><br>

<center>![Coffre_01](https://user-images.githubusercontent.com/35993911/69336646-48bd1880-0c5f-11ea-8007-b010bed4a853.JPG) ![Coffre_02](https://user-images.githubusercontent.com/35993911/69336728-7904b700-0c5f-11ea-9aa4-79ae264ea779.JPG)</center><br>
<center>Chest type lid</center><br>

##Software

This is an inkscape extension <br>
In order to install, unzip the downloaded file. You will need one interface file (either english or french is proposed) with .inx extension. You also will need the two program files, with the .py extension. Copy these 3 files into your inkscape extension directory. 
To locate this directory, you can use the Edit/Preferences command in inkscape.
You can choose either the global extension directory or your local one. You must be administrator to install the software for all users, it is not necessary for yourself.
For Linux users, it's ~/.config/inkscape/extensions for the local directory. With windows, it's in most cases C:\Users\Your_Name\AppData\Roaming\inskscape\extensions.  <br>


###User manual

The user interface use tabs, each tab is dedicated to a specific part. You should use the tabs in the given order, but it is not mandatory.
1. Dimensions tab. It gives the **inner** dimensions of the box. You can choose the unit, but only mm have been tested! Pay attention to the thickness of the material otherwise the notches will not fit well. I had materials that do not really respect their specifications (ex MDF 3mm which is 3.2mm thick). This sounds not very important, but it greatly hinders or even prevents assembly. The laser beam compensation input gives the "size"  that is removed by the laser. For wood, 0.1mm is a good value. For plexiglass or PMMA, mount to about 0.2mm otherwise the assemblies will be loose and require glue. <br>

<center>
![Onglet_Dimensions](https://user-images.githubusercontent.com/35993911/69336761-8fab0e00-0c5f-11ea-916b-4c8cdd9ac8fb.png)
</center><br>

2. Rounded corners tab. The first box makes it possible to force all the corners as rights. Alternatively, you can choose the radius of curvature of each corner independently. 0 indicates a right corner. Be careful not to put a value too low. Any value greater than 0 and less than 10 (approximately) should be outlawed. 

<center>![Onglet_CoinsArrondis](https://user-images.githubusercontent.com/35993911/69336767-93d72b80-0c5f-11ea-9c42-00ed50379fef.png)</center><br>

3. Cover style tab. The different lid styles were detailed in the previous paragraph. Choose the one that suits your use. Be aware that slide or hinged covers are incompatible with rounded corners at the back of the box. For chests, the 4 corners must be straight.
<center>
![Onglet_Couvercle](https://user-images.githubusercontent.com/35993911/69336771-976ab280-0c5f-11ea-92d0-d22e4161d1c7.png)</center><br>

4. Inner slots tab. The inside of the box can be divided into slots, you can set the number of columns and rows. Be aware that when one of these numbers greater than 1, the software generates an inner plate, to avoid having the notches on the visible faces. Do not be surprised if you have a few more faces. The size of the slots must be at least 20mm, you must respect this.

<center>
![OngletCasesInterieures](https://user-images.githubusercontent.com/35993911/69336801-a6e9fb80-0c5f-11ea-9f6f-d8ce6b19e5ce.png)</center><br>

5. Tab notches. You can give the size of the notches or finger joints by direction (X = length, Y = width, Z = height). You can also let the extension choose what is reasonable given the size of the box. <br>

<center>![OngletEncoches](https://user-images.githubusercontent.com/35993911/69336791-a3567480-0c5f-11ea-90db-360ee66d64c1.png)
</center><br>

## Future work

If you have exiting ideas about this extension, let me know!
I could help to design these new ideas, but you are also welcome to realize your own ideas. In any case, do not forget to publish your modifications and enhancements.

##Bibliography

I was inspired by the site of Florian Festi, very well done, but I tried to regroup various possibilities in one extension, and I also corrected some problems on the generated boxes .
Le The Florian Festi web site: [https://www.festi.info/boxes.py Festi.info]


