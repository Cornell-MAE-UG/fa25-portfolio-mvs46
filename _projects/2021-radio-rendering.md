---
layout: project
title: Wrench Design Project
description: CAD/ANSYS Project
technologies: [Autodesk Fusion, ANSYS]
image: /assets/images/straincontour.png
---

<br>
<br>
<br>
<br>
1: The following is my CAD model of the wrench.
<img src="./assets/images/CADb.png" alt="Alt Text" width="957" height="375.5">
<img src="./assets/images/CADh.png" alt="Alt Text" width="957" height="375.5">
<img src="./assets/images/CADL.png" alt="Alt Text" width="957" height="375.5">

2: The material I will be using is a Titanium alloy. The relevant mechanical properties of this material are:
Young’s Modulus: 13.1*10^6 psi (The maximum of the listed range on the database, which is the worst case scenario for the purposes of this analysis.)


Poisson’s Ratio: 0.31


Ultimate Strength: 135000 psi (minimum value which is worst case scenario for this analysis)


Fracture toughness: 80.1*10^3 psi*in^(½) (minimum value which is worst case scenario for this analysis) 

Fatigue Strength at 10^6 cycles: 70*10^3 psi (minimum value which is worst case scenario for this analysis) 

3: The loads and the boundary conditions in ANSYS:
<img src="./assets/images/0disp.png" alt="Alt Text" width="955" height="248">

4: <img src="./assets/images/straincontour.png" alt="Alt Text" width="1054" height="304">

5: <img src="./assets/images/pstresscont.png" alt="Alt Text" width="1054" height="304">

6: The Finite Element Method calculations gave a maximum normal stress of 67.386 ksi located on the boundary of the zero displacement condition. The hand calculations gave a maximum normal stress on the handle of 28.8 ksi. This value was supported in the FEM calculations as well. The load point deflection from the FEM calculations was 0.85803 inches. The hand calculated deflection was 0.75 inches. The reason for this discrepancy is the presence of geometry and boundary conditions not taken into account by the hand calculations. The presence of the fillets on the drive and stress singularities at the boundary of the clamped condition are the reason for the discrepancy. The strains at the strain gauge locations (one inch from the drive) from the FEM calculations were 2.061*10^-3 in the axial direction and -6.39*10^-4 in the two perpendicular directions. These values are also found by hand calculations. 

7: The torque wrench sensitivity using the strains from the FEM calculations and using a Wheatstone half bridge set-up was 2.06 mV/V. 

8: The strain gauge I selected is a linear strain gauge from DwyerOmega’s catalogue. It measures .3” x 0.228”. It fits on the handle of the wrench which measures 17” x .5” (16” length starting from the drive). 