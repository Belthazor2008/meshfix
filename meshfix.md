# sample output #
```
meshfix lh.stl -a 1 -n 1
Fixing asin tolerance to 1.745418e-02
\
INFO- Loaded 812004 vertices and 270668 faces.
0% done 
********* ITERATION 0 *********
Removing degeneracies...
INFO- Removed the smallest 2 of 3 shells
INFO- Removed the smallest 4 of 5 shells
Removing self-intersections (using advanced method)...
INFO- Stage: Remove and Fill (1)
INFO- 1635 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 106 of 107 shells
INFO- 1280 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 6 of 7 shells
INFO- 291 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 10 of 11 shells
INFO- 168 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 111 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 101 intersecting triangles have been selected (in selection).
INFO- Stage: Laplacian Smooth (1)
INFO- 118 intersecting triangles have been selected.
INFO- Laplacian smoothing of selected triangles.
INFO- Stage: Remove and Fill (7)
INFO- 159 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 11 of 12 shells
INFO- 148 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 45 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 9 intersecting triangles have been selected (in selection).
INFO- 9 intersecting triangles have been selected (in selection).
INFO- Stage: Laplacian Smooth (2)
INFO- 9 intersecting triangles have been selected.
INFO- Laplacian smoothing of selected triangles.
INFO- Stage: Remove and Fill (12)
INFO- No intersecting triangles detected (in selection).
INFO- No intersecting triangles detected.
********* ITERATION 1 *********
Removing degeneracies...
INFO- Removed the smallest 1 of 2 shells
Removing self-intersections (using advanced method)...
INFO- Stage: Remove and Fill (1)
INFO- 269 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 18 of 19 shells
INFO- 275 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 49 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- 35 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 2 of 3 shells
INFO- 15 intersecting triangles have been selected (in selection).
INFO- 7 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- Stage: Laplacian Smooth (1)
INFO- 13 intersecting triangles have been selected.
INFO- Laplacian smoothing of selected triangles.
INFO- Stage: Remove and Fill (7)
INFO- 8 intersecting triangles have been selected (in selection).
INFO- 10 intersecting triangles have been selected (in selection).
INFO- No intersecting triangles detected (in selection).
INFO- No intersecting triangles detected.
********* ITERATION 2 *********
Removing degeneracies...
INFO- Removed the smallest 1 of 2 shells
Removing self-intersections (using advanced method)...
INFO- Stage: Remove and Fill (1)
INFO- 49 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 3 of 4 shells
INFO- 33 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- No intersecting triangles detected (in selection).
INFO- No intersecting triangles detected.
********* ITERATION 3 *********
Removing degeneracies...
Removing self-intersections (using advanced method)...
INFO- Stage: Remove and Fill (1)
INFO- 7 intersecting triangles have been selected (in selection).
INFO- Removed the smallest 1 of 2 shells
INFO- No intersecting triangles detected (in selection).
INFO- No intersecting triangles detected.
Saving output mesh to 'lh_fixed.off'
```
# Differences produced by the self intersection removal (mesh of one hemisphere of a human brain) #
![http://dl.dropbox.com/u/2465545/altered_triangles.jpg](http://dl.dropbox.com/u/2465545/altered_triangles.jpg)