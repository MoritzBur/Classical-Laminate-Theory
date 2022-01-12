# Classical-Laminate-Theory

COMPATIBILITY: coded o CASIO fx-CG50. No other devices tested yet

USAGE:  copy text files to calculator memory via USB. CG50 will automatically convert int usable program files after disconnecting from USB

        run INITCLT to initialize all necessary matrices with their respective dimensions
        
        start program "CLTHEORY" to access main menu


WHAT IS IT?

Casio Basic Program to automate reocurring calculations:


Q'

-local stiffness matrix Q' from material properties: CALC'

-enter previously calculated local stiffness matrix: SETQ'

-save Q' as a material for further operations: Q'SVE


QTRF

-select saved material and enter ply angle

to give transformation matrix Tepsilon and transformed global stiffness matrix Q


ABD

-define laminate (materials, ply angles, thicknesses): LAYERS

to calculate ABD matrix a fuckload faster than by typing all that bullshit into a potatocalculator: CALCABD

(ABD is saved for further calculations)


STRAN (structural analysis)

-calculate either:

  -load vector from ABD and strains
  
 or:
 
  -strain vector from ABD and loads
  
(strain vector saved for further calculations)




POST (Postprocessing menu)

   select:
   
   -strains in specific z planes: GLOSTRAI
   
   -transformation of strains to local coordinate system epsilonk'(epsilonk,alphak): STRALOC
   
   -stresses from local strains: LOCSTRES

   TO BE CODED:
   
   -reserve factors for given stresses and strenghts: RF
   
   -stresses in specific z-planes
   
   -transformation of stresses into local coordinate systems




Note that most stuff is written in german, some english when things had to be shorter. Maybe somebody could make a polished english version?

The codes are deliberately split into small sections to be used in exams where this code might be used.

For real world application things culd be a lot shorter and more automated however.
