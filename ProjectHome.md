# Information #
http://www.ima.ge.cnr.it/ima/personal/attene/PersonalPage/attene.html#Software

# Description #
```
$ meshfix --help
MeshFix v1.2-alpha - by Marco Attene, Mirko Windhoff, Axel Thielscher.
================================================================================
USAGE: meshfix <file1> [<file2>] [OPTIONS]
  Processes file1 and saves the result to <file1>_fixed.off.
  An optionally passed file2 is merged with the first one.
OPTIONS:
 -a <epsilon_angle>  Allowed range: 0 < epsilon_angle < 2, default: 0 (degrees).
 -j                  Join 2 biggest components if they overlap, remove the rest.
 -jc                 Join the closest pair of components.
 -h, --help          Print this help and exit.
 --shells <n>        Only the n biggest shells are kept.
 -o <output>         Set the output filename (without extension).
 -q                  Quiet mode, don't write much to stdout.
 --remove-handles    Remove all handles of the mesh.
 -u <steps>          Uniform remeshing of the whole mesh, steps > 0
   --vertices <n>    Constrain number of vertices to n (only with -u)
 --no-clean          Don't clean.
 --smooth <n>        Apply n laplacian smoothing steps.
 -s, --stl           Result is saved in STL     format instead of OFF.
 -w, --wrl           Result is saved in VRML1.0 format instead of OFF.
 --fsmesh            Result is saved in FreeSurfer format instead of OFF.
 --xshift <d>        Shift x-coordinates of vertices by d when saving output.
                     Only works with --fsmesh; used to deal with small FreeSurfer glitch
 --msh               Result is saved in gmsh format for debugging (including vertex and triangle masks)
 == Cutting, decoupling, dilation ==
 --cut-outer <d>     Remove triangles of 1st that are outside of the 2nd shell.
 --cut-inner <d>     Remove triangles of 1st that are inside  of the 2nd shell.
                     Dilate 2nd by d; Fill holes and keep only 1st afterwards.
 --decouple-inin <d> Treat 1st file as inner, 2nd file as outer component.
                     Resolve overlaps by moving inners triangles inwards.
 --decouple-outin <d> Treat 1st file as outer, 2nd file as inner component.
                     Resolve overlaps by moving outers triangles inwards.
 --decouple-outout <d> Treat 1st file as outer, 2nd file as inner component.
                     Resolve overlaps by moving outers triangles outwards.
                     Constrain the min distance between the components > d.
 --fineTuneIn <d> <n> Used to fine-tune the minimal distance between surfaces 
                     A minimal distance d is ensured, and reached in n substeps 
                     When using the surfaces for subsequent volume meshing by gmsh
                     this step prevent too flat tetrahedra
 --fineTuneOut <d> <n> Similar to --fineTuneIn, but ensures minimal distance in the other direction
 --dilate <d>        Dilate the surface by d. d < 0 means shrinking.
 --intersect         If the mesh contains intersections, return value = 1.
 --intersect -o fname.msh  If the mesh contains intersections, return value = 1.
                     In addtion, save mesh with highlighted intersections in Gmsh format
Accepted input formats are OFF, PLY and STL.
Other formats are supported only partially.
See http://jmeshlib.sourceforge.net for details on supported formats.

If MeshFix is used for research purposes, please cite the following paper:
M. Attene - A lightweight approach to repairing digitized polygon meshes.
The Visual Computer, 2010. (c) Springer.
```

# Building #

http://windhoff.net/wiki/how_to/build_meshfix_on_ubuntu_linux_64bit