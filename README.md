# 60mm Toy Drone Body Replacement

This is a body for a toy drone of unknown origin that I received as a Christmas present. It was sold by Sharper Image and came with a body in the shape of an F16 fighter. Basically a generic toy drone. Predictably, I took the plastic body off of it and eventually broke one of the motor mounts on a tree. There are no replacement parts that I can find, so I decided to make my on using my 3D printer. This model should fit on most 3D printers. It's about 140mm to the sides and 168mm diagonally. 

The propellers are 60mm long and the motors are 8.5mm x 20mm. I tried to keep the motor leads as short as possible and they fit fine using the model that I retrofitted. Motor leads need to be at least 60mm long. The model that is supplied with this archive should be usable in most situations, but it can easily be modified to meet more specific needs. My version of the model weighed in at about 25g without motors, battery or electronics. That's less than half of the original. The model flies quite well as a result.

### Modifying the model

The model is created using FreeCad, which is a cross-platform 3D CAD toolbox that is fairly complete and perfectly suitable for creating models for printing on a 3D printer. A tutorial on how to use FreeCad is beyond the scope of this readme, but there is lots of information out on the web and it's not hard to learn, once you figure out what to do. This is a tutorial that describes what to do. 

The printable model, named **body.amf,** is composed of smaller 2D drawings (DXF drawings created with QCAD) that are basically extruded to different lengths in FreeCad. The smaller drawings are then overlaid on a single drawing and then bound into a single shape. Each of the smaller DXF drawings is loaded into FreeCad separately. The location and size of each component is placed in such a way as to allow simply copy/paste and there is no need to move things around. For very simple changes, each drawing can be manipulated separately and then combined in FreeCad. To make bigger changes, such as changing the placement of the motors, one would be better off to redray everything in a 2D cad application and then separate the individual components as illustrated by this archive. This is easier than it sounds.

1. Create a box the size of the general outline
2. Place circles that represent the propeller arc inside the box in the layout that you want. 
3. Fill in the details from there. Take a look at **layout.dxf** to see an early version of the final model. I didn't bother to propagate changes back to this drawing because I don't feel that it's needed. But this will serve to illustrate what I mean by filling in the details.
4. Take the overall drawing that you have created and then divide it up into smaller ones. Remember that you will need to print it and so you do not want to use supports unless it's absolutely necessary.

### The 2D drawings

In general, the DXF is loaded into FreeCad and then the closed surfaces are converted to a "face" using the Draft toolbox. Then, parts of the drawing that need to be removed are subtracted with the Part toolbox.

#### motors

This drawing has the motor mounts. They are a split ring that is intended to grip the motor near its center. I used a dab of hot glue to secure it in place. The DXF file is loaded into FreeCad and each motor mount is extruded to +6mm height. 

#### shroud

This is the fan shroud that protects the propellers from damage. It does not really help produce thrust. These are extruded to +16mm height and then the centers are subtracted from the outer shell. 

#### brace

This is the part of the motor mount that connects the motors physically to the rest of the frame. It also connects the shrouds to the rest of the frame. The brace is extruded to +2mm.

#### base

This is the part that holds the whole thing together. The electronics and the battery mount to the base. Actually mounting the electronics on the base is left up to the builder. What I did was simply use a dab of hot glue to hold things together. The base is extruded to +1mm. The subtract the rectangular holes.

### Combine the models

To combine the models, you simply copy them from the original (Ctrl-C) and paste them into a new model. (Ctrl-V) It is important to remember that these will already be in the proper locations. Do not move them unless you have a good and specific reason for doing it. 

