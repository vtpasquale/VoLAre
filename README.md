![alt text](http://aricciardi.weebly.com/uploads/7/5/7/7/7577137/3149314.png?501.png "Vortex Lattice for Aeroelasticity (VoLAre)")

Vortex Lattice for Aeroelasticity (VoLAre) is a vortex lattice code that solves steady three-dimensional potential-flow aerodynamic trim problems.  VoLAre was created to provide nonlinear aeroelastic trim analysis that was needed for methods research in aeroelastic scaled-model design [1-2].  

General-purpose commercial aeroelastic codes (e.g., Nastran) support aeroelastic trim, but not with nonlinear structures.  The research version of VoLAre was paired with custom spline tools and interfaced with Nastran for nonlinear aeroelastic trim analysis.  Implementation details are provided in [3]. 

This publically-released version of VoLAre is significantly modified from the research version.  The main differences are:
1. [ZAERO]( https://www.zonatech.com/zaero.html)-formatted input is used for model definition.  Download and reference the ZAERO User’s Manual from ZONA Technology, Inc. while reading through VoLAre’s example input files. 
2. Trailing vortices now remain in the planar reference surface rather than curving along the mean camber surface. This choice significantly reduces the computational cost of calculating induced velocities while having a negligible impact on accuracy for most cases.  
3. Splining and aeroelastic coupling are not implemented yet.

References
============

1. Ricciardi, A. P., Canfield, R. A., Patil, M. P., and Lindsley, N., ``Nonlinear Aeroelastic Scaled-Model Design,'' doi: [10.2514/1.C033171]( https://dx.doi.org/10.2514/1.C033171). Journal of Aircraft, Vol. 53, No. 1 (2016), pp. 20-32.
2. Ricciardi, A. P., Eger, C. A. G., Canfield, R. A., Patil, M. P., and Lindsley, N., ``Nonlinear Aeroelastic Scaled-Model Optimization Using Equivalent Static Loads,'' doi: [10.2514/1.C032539]( https://dx.doi.org/10.2514/1.C032539). Journal of Aircraft, Vol. 51, No. 6 (2014), pp. 1842-1851.
3. Ricciardi, A.~P., ``Geometrically Nonlinear Aeroelastic Scaling,'' [Ph.D.~Dissertation](http://hdl.handle.net/10919/24913), Virginia Tech, December 2013.
