# Computer Numerical Craft
Computer Numerical Craft is a explorations at the intersection of digital fabrication and craft techniques. Specifically, I am exploring workflows around ceramics and CNC machines. So far I've experimented with slip casting paired with 3D printing, slab building paired with laser cutting, and press molding paired with CNC routing. 

This work was created by Hillary Predko of [Desire Line Design](https://www.desireline.ca/) for [the Open Hardware Summit 2026](https://2026.oshwa.org/) at [Hamilton Craft Studios](https://hamiltoncraftstudios.com/).

## Slip Casting x 3D Printing

From [Digital Fire](https://digitalfire.com/glossary/slip+casting):

> Slip casting is the forming of ceramics by pouring or pumping deflocculated (water-reduced) clay slurry, called casting slip, into plaster molds. In the process, the absorbent plaster pulls water from the slurry, and over a period (e.g. 20 minutes) a layer builds up against the mold surface. The slurry is then poured out and, as the item stiffens it shrinks slightly and pulls itself away from the mold enabling removal.

I've been trying on and off to make slip cast ceramics from 3D printed forms for a few years. I've primarily been inspired by [Hammerly Ceramics](https://www.hammerlyceramics.com/?srsltid=AfmBOooTg6y697EVtHqCTvBsQcPU8A-xh-ib0O3oRq0D_y5tCeebTc0j) who makes these beautiful intricate forms. I am still many years away from achieving similar results.

After producing a bunch of work that I was not really happy with, I decided to make a teeny tiny mold to make small pieces for glaze testing (and easier transporation of the finished work to Germany). 

<img width="300" height="400" alt="PXL_20260320_224926714" src="https://github.com/user-attachments/assets/6c84d13a-0f86-4803-9139-6c448a8d7602" />
<img width="300" height="400" alt="PXL_20260320_181734010" src="https://github.com/user-attachments/assets/27dbfc20-78d5-454f-b10a-88bec6d2ac66" />

I've been making simple one part molds, which means I design and print a positive of the object I want in ceramic then pour plaster over it. To make a one part plaster mold, you will need to CAD a shape with no undercuts, which conveniently works well with FDM printing. I've been experimenting with making undulating patterns on the sides of vessels. Once you have the vessel shape you want, I add a cylinder with a draft angle to the top to act as a reservoir for the slip. I use an [online calculator](https://plaster.glazy.org/) to estimate how much plaster to mix and pour for my molds.

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/db1db927-bd8c-4691-9443-e0fc67aaa5c2" />
<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/cbbde29a-8e51-46d4-96ea-f4f827dbf236" />

Ideally I would print the models at the highest quality setting, but all of my experiments were made before I had a 3D printer. To minimize the appearance of the layer striations, I coat the print in XTC-3D by Smooth On, a finishing resin for 3D prints. Then comes several rounds of sanding and coating.

While some people 3D print the mold exterior, I decided to save time by using scrap melamine sheets. I screwed this together to make a water tight box before coating everything in Murphy's Oil Soap as a mold release.
I use #1 Pottery Plaster and demold after ~1 hour.

Plaster molds need to dry for several days or up to a week before they can be used for slip casting. Once the plaster no longer feels clammy, you're ready to get started.
Pour slip into the mold and wait for 15-30 minutes (you'll be able to see the wall thickness) before pouring it out.

<img width="300" height="400" alt="PXL_20260506_174539612" src="https://github.com/user-attachments/assets/2361f884-6ce4-49ec-be87-6becebb23b7b" />


## Slab Building x Laser Cutting

From [JJ Clay Studio](https://www.jjclaystudio.com/slab-built-definition-comprehensive-guide-to-foundations/):
>Slab built definition refers to a method in pottery where clay is rolled into flat sheets and then assembled to create various forms, allowing for limitless creativity and unique textures that wheel-thrown pieces often lack. This ancient technique has been embraced by artists for centuries, celebrated for its versatile nature and capacity to produce functional and decorative ware.

I created a series of surfaces in Rhino with top to bottom ratios of 1:1 1.5:1, 2:1. I drew two curves that were lofted to create the surface.
These were then transferred to 2D templates using the UnrollSrf command, which flattened 3D objects. Using DupEdge, I created outlines for SVG templates that could easily be lasercut. 

<img width="827" height="413" alt="image" src="https://github.com/user-attachments/assets/838f088d-a302-421b-9010-e82b7527db0d" />

Bonus round before laser cutting! I drew designs on the 1:1 template and distorted them to fit the other templates using FlowAlongSrf. These then became lasercut stencils for the vessels.
Unfortunately, getting perfectly tessellated stencils to sit flat against my imperfect pottery was beyond my skill at hand building.

I used roofing tar paper to laser cut waterproof reusable templates. However, I could not confirm from the SDS that this material is absolutely safe to cut. There are many examples of people selling laser cut templates with this material, and I am using my own machine with ventilation so I took the risk. You might be more cautious than me.

Your templates are now ready to use! In my shop we have a slab roller that flattens clay to a uniform thickness, but otherwise you can use spacers to roll out uniform slabs by hand.
Balancing the thickness of the slab with the size of the template was something of a challenge - I did not manage to create vessels exactly the same size as my CAD models making stencils challenging.

<img width="400" height="300" alt="PXL_20260414_192149868" src="https://github.com/user-attachments/assets/248fef0d-6e17-48ff-8917-263375f69561" />
<img width="300" height="400" alt="PXL_20260408_193202419" src="https://github.com/user-attachments/assets/8dcbf0bf-1cfb-46e8-9520-84f852a76413" />

I also designed a template to make a replica Raktajino mug from DS9, which is extremely silly and definitely not a stellar mug from a holding liquids perspective.

<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/c09a2243-c397-4ce8-b527-fed7b63a6e15" />
<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/a7f03f91-d300-4215-bf5a-fa124df81074" />



## Press Molding x CNC Routing

From [Spruce Crafts](https://www.thesprucecrafts.com/using-press-mold-tips-and-tricks-4091260):
>In pottery, press molding refers to the process in which clay is forced into a mold in order to take on a certain shape. Once the mold is removed, the piece produced is a uniform replication of the inside of the mold (similar to casting with metalwork). Press molds work great when reproducing multiple pieces of ceramics—from bowls to plates to tiles.

I used 2D SVGs along with angled V-bits on a CNC router to create bevelled surfaces from MDF and plaster. I was pretty experimental creating 2D vector drawings to turn into molds. Since I was primarily using MDF, I didn't want anything that was too detailed because I wasn't sure the cuts would be sharp.
I used a 120° v-bit with a profile toolpath to create 3D geometry from flat vectors.

<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/324a49ec-fb9e-418e-883d-5515286228ed" />

After the patterns were cut into MDF sheets, I cut 3D forms that the pressed clay could be draped over while it dried. These were cut with a 1/2" ballnose bit then coated in wood filler and sanded.
All of the MDF pieces were finished in multiple coats of polyurethane to limit water absorption.

I coated the molds with corn starch before as a mold release before getting started. I then rolled out slabs of clay that were slightly thicker than the molds and pressed it in with a soft rib. Getting it out is not exactly easy - I had the best results if I used a hair dryer to dry the clay before slowly coaxing it out.

<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/ce71b43c-0a1d-4b90-883c-9228a01ca994" />

Ultimately MDF is not the best material for these molds. If left uncoated, it would absorb too much water and deteriorate. Coated in polyurethane, the clay couldn't dry evenly and became somewhat stuck.
I did try machining partially set plaster with the SVG geometry projected onto the 3D geometry. The results were quite nice but the process was extremely messy.

<img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/44764612-015c-4ab4-b366-a0db7847e3b5" /><img width="300" height="400" alt="image" src="https://github.com/user-attachments/assets/e7450db3-ab48-4595-9bd4-411e1a9ea846" />



