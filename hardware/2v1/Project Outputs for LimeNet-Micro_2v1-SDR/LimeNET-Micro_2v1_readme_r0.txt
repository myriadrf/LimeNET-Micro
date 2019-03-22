Board Description
-----------------

board designation           : LimeNet-Micro
board version		        : v2.1
board type                  : Lead Free
board size                  : 75 mm x 143 mm
board with frame size		: 105.4 mm x 173.4 mm
board thickness             : 1.6 mm +/- 10 %
board material              : IT-180A preferred or equivalent RF-rated material (up to 3 GHz or higher)
number of layers            : 6 (4 inner)
 
Stackup:
	Via nr.		Via type		Drill diameter			Ring diameter		Additional specs./Info
		#1		Throughole			0.2 mm					0.4 mm	
		#2		Throughole			0.4 mm					0.8 mm
		#3		Throughole			0.2 mm					0.35 mm			In pad. Resin filled with metal cap (IC1)
		#4		Throughole			0.2 mm					0.5 mm			Via under IC1 thermal pad. They should not be plugged. Other 0.2mm drill 0.4mm  
																			ring vias under IC1 thermal pad must be plugged
		
 
Top layer copper foil thickness: 17.5 um
Dielectric thickness between Top layer and 2nd layer: 173 um (6.8 mils)
Dielectric between Top layer and 2nd layer relative permittivity (Er): 4.2

Bottom layer copper foil thickness: 17.5 um
Dielectric thickness between L5 layer and Bottom layer: 173 um (6.8 mils)
Dielectric between L5 and Bottom layer relative permittivity (Er): 4.2


minimum finished hole size  :  200 um
minimum spacing             :  100 um
minimum track width         :  100 um

drill diameters             : finished hole

plating finish (both sides) : immersion gold
                              0.05-0.10 um of gold over
                              2.50-5.00 um of nickel
							
Top silkscreen              : Required
Bottom silkscreen           : Required


Drill files
-----------------
	- LimeNet-Micro_2v1.DRR -> Drill report detailing the tool assignments, hole sizes, hole count and tool travel. 
   
	- Throughole vias are covered in the following files:
   								File Name																	Start Layer						Stop Layer
						LimeNet-Micro_2v1-RoundHoles.TXT														Top								Bottom
    - Slotholes are covered in the following files:
						LimeNet-Micro_2v1-SlotHoles.TXT															Top								Bottom	
						
	- IMPORTANT! Hole diameters are final manufactured diameters INCLUDING HOLE METALIZATION.
	
Gerber files
---------------

			File Name					Layer/Comment
		LimeNet-Micro_2v1.GTL				Top (Signal)
		LimeNet-Micro_2v1.G1				L2  (Signal)
		LimeNet-Micro_2v1.G2				L3  (Signal)
		LimeNet-Micro_2v1.G3				L4  (Signal)
		LimeNet-Micro_2v1.G4				L5  (Signal)
		LimeNet-Micro_2v1.GBL				Bottom (Signal)

		 
		LimeNet-Micro_2v1.GPB				Bottom Pad Master
		LimeNet-Micro_2v1.GPT				Top Pad Master

		LimeNet-Micro_2v1.GTO				Top Overlay
		LimeNet-Micro_2v1.GTP				Top Paste
		LimeNet-Micro_2v1.GTS				Top Solder

 
		LimeNet-Micro_2v1.GBS				Bottom Solder
		LimeNet-Micro_2v1.GBP				Bottom Paste
		LimeNet-Micro_2v1.GBO				Bottom Overlay


		LimeNet-Micro_2v1.GM1				Mechanical 1 (Board Cutout and dimensions)
		LimeNet-Micro_2v1.GM6				Notes (Board shape)
		

		LimeNet-Micro_2v1.GM14				ASM BOT (Assembly bottom)
		LimeNet-Micro_2v1.GM15				ASM TOP (Assembly top)
		
  
Important Notes
---------------
All 0.2mm vias including 0.35mm ring and 0.2mm drill via-in-pads must be resin filled with metal cap (IC1).

IC1 thermal pad vias with 0.4mm ring and 0.2mm drill must be resin filled with metal cap.

IC1 thermal pad vias with 0.5mm ring and 0.2mm drill must be left open (NO resin fill with metal cap). 4 vias in total, marked with note in mechanical 1 (*.GM1) gerber file.

DRCs must be run on Gerber files before building boards.

All through hole vias may be plated shut.

Solder mask : dark blue, both sides, halogen free, glossy finish (NOT matte).

Silkscreen : white epoxy ink, halogen free, both sides. No silkscreen on pads.

Electrical test : 100 % netlist.

Boards are to be individually bagged.

Design software used:  Altium Designer 18.1.9 (build 240)

Controlled Impedance
--------------------

  * 50 Ohm microstrip line (Top layer) characteristics:
    Top layer copper foil thickness: 17.5 um
	Track width = 0.325 mm (12.795 mils)
	Dielectric thickness from top to L2 = 173um (6.8 mils)
	Dielectric between Top layer and 2nd layer relative permittivity (Er): 4.2
	
	Approximate microstrip line impedance = 49.99 Ohms (+/- 10% tolerance)

  * 50 Ohm microstrip line (Bottom layer) characteristics:
    Bottom layer copper foil thickness: 17.5 um
	Track width = 0.325 mm (12.795 mils)
	Dielectric thickness from Bottom to L5 = 173um (6.8 mils)
	Dielectric between Bottom layer and L5 relative permittivity (Er): 4.2
	
	Approximate microstrip line impedance = 49.99 Ohms (+/- 10% tolerance)	
	
  * 100 Ohm coupled microstrip line (Top layer, RF) characteristics:
    Top layer copper foil thickness: 17.5 um
	Track width = 0.2 mm (7.87 mils)
	Track spacing = 0.14 mm (5.51 mils)
	Track width/spacing ratio = 1.428
	Dielectric thickness from top to L2 = 173um (6.8 mils)
	Dielectric between Top layer and 2nd layer relative permittivity (Er): 4.2
	
	Approximate coupled microstrip line impedance = 100.752 Ohms (+/- 10% tolerance)	
	
  * 100 Ohm coupled microstrip line (Bottom layer, HDMI) characteristics:
    Bottom layer copper foil thickness: 17.5 um
	Track width = 0.2 mm (7.87 mils)
	Track spacing = 0.14 mm (5.51 mils)
	Track width/spacing ratio = 1.428
	Dielectric thickness from L5 to Bottom = 173um (6.8 mils)
	Dielectric between L5 layer and Bottom layer relative permittivity (Er): 4.2
	
	Approximate coupled microstrip line impedance = 100.752 Ohms (+/- 10% tolerance)	