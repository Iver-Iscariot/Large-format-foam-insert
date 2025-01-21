Making a custom trunk to carry my large format camera, with a fitted foam padding on the inside

CAD file of my camera 
![image](https://github.com/user-attachments/assets/add5209d-44c2-4111-9af3-86e1e899c17b)
Its a cambo monorail-type large format camera

I have modelled all the components, and laid them out in a desirable, ergonomic layout (Things can be accessed in the order of when you assemble them (this was a issue with the case i bought it in)).
I then drew some simple box-envelopes around them, such that they have some tolerance. These envelope-boxes are also in increments of 5mm height wise, as this is limited by the foam i will be using.

On that, it was hard to find a supplyer of (laser cuttable) foam in norway, but i ended up with this from rufo
https://www.rufo.no/products/50-mm-plastazo3
Its a laminate of 5mm foam layers that can be pulled apart.

Originally, I wanted to fit this in a peli-case with a suitcase-style pullbar and wheels, but there was no way this would fit. Especially since i wanted to store the camera semi-assembled in the camera (it typically takes ~20min to take ONE picture with this camera, so every time-save is worth it)
I will therefore simply lasercut a dovetail-plywood box for it, and install some hardware.
To make it suitcase-style, i will use a "sekketralle" from clas ohlson
https://www.clasohlson.com/no/Sammenleggbar-tralle/p/40-8867
I will lasercut some plywood pieces matching the pattern on the bottom, so that it can be slotted onto it (and attached to the handle bar with some sort of straps) I need to use the sekketralle for other stuff, and it is practical to be able to remove the trunk and carry as a backpack with some sort of straps, if you're shooting in rugged terrain

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
EDIT: Making the inside purely out of foam would be VERY expensive. I therefore pivoted to making inside walls, and put padding on them 
![image](https://github.com/user-attachments/assets/ac27a6ac-4c31-41f5-b760-39f09100990a)

I use boxes.py to generate the lasercut-files using this text carefully calculated from my cad file
https://boxes.hackerspace-bamberg.de/TrayLayout?

```
Height: 224 (230 - width)

Uncheck "outside" (da er målene under størrelsen på rommene, som var det jeg målte i cad-filen)
211:31:184:66:71:84
32:115:14:133:49:32


 ,> 211.00mm
 | ,> 31.00mm
 | | ,> 184.00mm
 | | | ,> 66.00mm
 | | | | ,> 71.00mm
 | | | | | ,> 84.00mm
+-+-+-+-+-+-+
|   | | | | |  32.00mm
+   + + + +-+
|   | | | | |  115.00mm
+   +-+-+-+ +
|   | |   | |  14.00mm
+ +-+ +   + +
| | | |   | |  133.00mm
+ +-+-+-+-+ +
|         | |  49.00mm
+   +-+-+-+-+
|   |     | |  32.00mm
+-+-+-+-+-+-+

Sett thickness til 6

Jeg må gjøre litt prøving og feiling for å finne en bra burn correction til mitt materiale før jeg kutter the big one
```

Høyden her er gitt ut ifra standardene, som er de høyeste/bredeste tingene som skal med. Boksen er derfor litt høy for resten av objektene. Jeg tenker å løse dette ved å lage små stilaser i boksene, som holder en bit med foam på riktig høyde, og som så holder foam med et cutout til objektet som holder det på plass. Treet som holder skummet må ha tilsvarende cutout, men med litt margin, slik at ikke objektet støter mot det
![image](https://github.com/user-attachments/assets/d92ed9e0-c2b1-4a3e-a579-bf8803b57c5e)



Lokket er helt likt, bare speilvendt, 69-6 = 63 mm høyt, og med de indre veggene i delen med små-rom fjærnet, slik at én stor skumplate kan holde alt nede

```
Height: 63 (69 - width)

Uncheck "outside" 
84:71:66:184:31:211
32:115:14:133:49:32


 ,> 84.00mm
 | ,> 71.00mm
 | | ,> 66.00mm
 | | | ,> 184.00mm
 | | | | ,> 31.00mm
 | | | | | ,> 211.00mm
+-+-+-+-+-+-+
|       |   |  32.00mm
+       +   +
|       |   |  115.00mm
+       +   +
|       |   |  14.00mm
+       +-+ +
|         | |  133.00mm
+       +-+ +
|       |   |  49.00mm
+       +   +
|       |   |  32.00mm
+-+-+-+-+-+-+


thickness 6
```
