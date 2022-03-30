# Classical-Laminate-Theory

### WHAT IS IT?

Casio Basic Program to automate reocurring calculations:

## little preview video: 
* enter local stiffness matrix 
* transformation to global stiffness matrix using ply angle

https://user-images.githubusercontent.com/40000888/149094070-ce522289-de91-486b-ae18-aacb72d040c5.mp4

### COMPATIBILITY: 
coded on CASIO fx-CG50. No other devices tested yet

### USAGE:
#### first usage / installation
   * copy text files to calculator memory via USB. CG50 will automatically convert into usable program files after disconnecting from USB.
   * for further information see [CG50 users guide](https://support.casio.com/en/manual/004/fx-CG50_Soft_v360_EN.pdf) chapter 13.1
   * Go to the "Programs" menu on your calculator
    * start Program INITCLT to initialize all necessary matrices with their respective dimensions. (this step is only necessary before first use or if you "broke" the setup while doing matrix calculations manually)    
#### normal usage      
   * start program "CLTHEORY" to access the main menu
   * enjoy


# Overview

Using the Programs should be self explanatory once you are familiar with common notation.
This is a non complete list of what the separate programs can do for you.

### Q'
* local stiffness matrix Q' from material properties: CALC'

* enter previously calculated local stiffness matrix: SETQ'

* save Q' as a material for further operations: Q'SVE



### Q (QTRF)

* select saved material and enter ply angle to give transformation matrix Tepsilon and transformed global stiffness matrix Q


### ABD

* asks if you already defined and saved your local layer stiffness as material; redirects to Q' if you still need to define materials
* define laminate (materials, ply angles, thicknesses): redirects to LAYERVEC
        (note: ply angle transformation will be handled automatically; no need to use "Q" prior to "ABD")
* to calculate ABD matrix a fuckload faster than by typing all that bullshit into a potato-calculator: redirects to CALCABD
* (ABD Matrix is saved for use in further calculations)


### Strukturanalyse/Structural analysis (STRAN)

* calculate either:

   * load vector from ABD and strains
  
     or:
 
    * strain vector from ABD and loads
  
(strain vector saved for further calculations)


### POST (Postprocessing menu)

   select:
   
   * strains in specific z planes: GLOSTRAI
   
   * transformation of strains to local coordinate system epsilonk'(epsilonk,alphak): STRALOC
   
   * stresses from local strains: LOCSTRES

### TO BE CODED:
   
   * reserve factors for given stresses and strenghts: RF
   
   * stresses in specific z-planes
   
   * transformation of stresses into local coordinate systems


Note that most stuff is written in german, some english when things had to be shorter. Maybe somebody could make a polished english version?

The codes are deliberately split into small sections to be used in exams where this code might be used.

For real world application things could be a lot shorter and more automated however.
