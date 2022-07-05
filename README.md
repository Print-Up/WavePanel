![Wave Panel Banner](https://user-images.githubusercontent.com/58088168/177226130-31179d59-6ae7-40d7-b497-12af1b72c2ec.jpg)

# Wave Panel
The Wave Panel is an open-source acoustic treatment solution that combines diffusion and absorption into one 3D printable panel. 

## About the Wave Panel
The Wave Panel is designed to be a fairly low-cost solution to tackle basic room acoustic issues. Acoustic treatment can cost anywhere from £10 for ugly looking foam to £100s for aesthetically pleasing solutions. 

Wave Panel costs around £10 per 250mm panel and offers the unique computer aided design cues offered by exposed 3D printed infill patterns. 

### Absorption
Absorption in the Wave Panel is handled by an insert of 25mm thick rockwool (or similar material) covered by a thin layer of acoustically transparant fabric for a splash of colour. 

### Diffusion
Diffusion in the Wave Panel is handled by the creation of 3D printed infill patterns. The infill pattern chosen is completely up to the user and can be configured in your slicer using the provided .3mf files. These .3mf files contain both the main Top Panel and the INFILL AREA model in the correct position. Each pattern will have it's own diffusion characteristics and once our research has been completed this will be available in the research section.

For information on how to configure your slicer for exposed infill, see the <b><i>Infill</b></i> section

## BOM (Bill Of Materials)
<i>Please Note: Calculate how many panels you require before purchasing any materials. Once you have this figure, multiply each item in your bill of materials with the number of panels.</i>
- 4x M3 x 16 SHCS
- 4x M3 Heat Set Insert (should be no deeper than 5mm) 
- 4x 6x3mm Magnet
- 245.6mm x 224mm x 25mm Rockwool (or similar)
- 300mm x 224mm of Acoustically Transparant Material - Colour/style doesn't matter.
- 4x T10 (Torx) 3.5mm x 19mm Self Tapping Countersunk Screws 
- 270g of ABS/ASA/PETG Filament - <i>Please Note: This value is an approximation based on a 0.4mm Nozzle, 3 Perimeters, 40% Gyroid Infill, 5 Bottom Layers, 6 Top Layers - Your mileage may vary!</i>

### Equipment Required
- A 3D printer with the correct bed size for your chosen panel.
- A soldering iron (for heat set inserts)
- A drill/impact driver with a T10 bit.
- M3 Screwdriver/Allen Key
- Superglue (for the magnets)
- A knife
- Scissors
- Ruler/tape measure
- Spirit Level

## Printable Parts
Each size variant contains 2 printable files:
- TopPanel
- BottomPanel

<p>The <b><i>Top Panel</i></b> is the part that will attach to the bottom panel (once mounted on the wall and filled with treatment) and also contains your model for infill creation. This model with its infill will serve as 'diffusion'. See the guide on how to configure your slicer for this.</p>


<img width="500" alt="Top Panel Infill Visualisation Image" src="https://user-images.githubusercontent.com/58088168/177223971-b072c6ab-f17c-4f7d-9878-7431081b8b0f.jpg">


The <b><i>Bottom Panel</i></b> is the part that attaches to the wall and holds your acoustic treatment materials.


<img width="500" alt="Bottom Panel Visualisation Image" src="https://user-images.githubusercontent.com/58088168/177224208-e4385726-5d77-4472-afa6-5405f0ffbe13.jpg">

## Infill Configuration
Configuring the infill object is a fairly simple task. The current guide only lists steps for PrusaSlicer and a Cura guide will be coming soon!

<ol>
  
<li>Import the .3mf Top Panel file you require.
  
<ul>
  
  <li>When importing this a pop-up warning will appear. This warning will mention <i>Multi-part Object Detected</i>. Please click **YES** to import the models correctly at their respective positions as **1 object with 2 sub-objects**. Clicking no will result in the part being split into 2 separate objects which will cause incorrect slicing. 
    
</ul>
     <p></p>
<img width="261" alt="Screenshot 2022-07-05 at 12 13 22" src="https://user-images.githubusercontent.com/58088168/177315965-32c0f787-3fac-489e-a6cb-65c5a93d96b0.png">

 <li>Select the <b>**INFILL_AREA**</b> object in the part list. This will also highlight in plater.
      <p></p>
<img width="800" alt="Screenshot 2022-07-05 at 12 20 37" src="https://user-images.githubusercontent.com/58088168/177316674-951c9a15-9d83-47f5-af96-cdc45d52afb5.png">
  <li>Right Click the <b>**INFILL_AREA**</b> object in the part list and select **Infill**
       <p></p>
<img width="261" alt="Screenshot 2022-07-05 at 12 23 58" src="https://user-images.githubusercontent.com/58088168/177316949-f6e3250d-1660-45cc-bc98-09b606cc3f05.png">

 <li>Right Click the <b>**INFILL_AREA**</b> again in the part list and select **Layers & Perimeters**
   <p></p>

 <img width="261" alt="Screenshot 2022-07-05 at 12 25 10" src="https://user-images.githubusercontent.com/58088168/177317122-4f14e805-1fda-4c21-b236-9df406daa7ae.png">
    
<li>Now select the modifier for the **INFILL_AREA** object. This will contain the two modifiers we just added (Infill and Layer & Perimeters). Navigating just below this when selected will show the options for these parameters. For a nice Gyroid Infill Diffuser an example of the settings are below:
   <p></p>
 <img width="261" alt="Screenshot 2022-07-05 at 12 30 27" src="https://user-images.githubusercontent.com/58088168/177320293-5e12b7e2-4978-4fd4-b969-4927b6f1ebff.png">
  <p></p>
<ul> <b>INFILL</b>
  <p></p>
  <li>Infill Density = 4% <i>(you can type this manually - you don't have to use the values in the dropdown box)</i>
  <li>Fill Pattern = Gyroid
</ul>
<br>
  <ul> <b>LAYERS & PERIMETERS</b>
    <p></p>
        <p>Here we want to entirely disable top & bottom layers as well as all perimeter printing. We **only** want the infill.</p>
    
<li> Bottom solid layers = 0
<li> Perimeters = 0
<li> Top Solide Layers = 0
</ul>
<li> Printing Time!
  <p></p>
  <img width="500" alt="Screenshot 2022-07-05 at 13 22 14" src="https://user-images.githubusercontent.com/58088168/177327326-4360ef65-01f9-45ca-b093-2d74e6d5f7a0.png">
</ol>

## Contact
<ol>
<li> Print Up
<ul> 
<li>info@printup.xyz
</ul>
<li> Main Contributor - Ben Weatherill
<ul>
<li>Discord: Phalnix#3899 - https://discordapp.com/users/phalnix#3899
<li>Email: ben@printup.xyz
</ul>
</ol>
