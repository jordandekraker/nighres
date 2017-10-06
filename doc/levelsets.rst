.. _levelsets:

Levelsets
==========

Levelsets are used in nighres as the main way to represent surfaces. They are signed distance functions in volume space, giving the distance to the surface boundary for every point in the image (by convention negative inside the object, positive outside, zero on the surface itself).

Levelsets can be converted to mesh structures by (connectivity consistent) marching cubes, and have useful properties for surface evolution via geometric deformable models (GDM)[1], ensuring regular sampling, and combining volume and surface information.

.. todo:: What is a levelset and why is Nighres using it, example of creating
   levelset using :func:`nighres.surface.probability_to_levelset`
   
References
Han et al., 2004 CRUISE: Cortical reconstruction using implicit surface evolution, NeuroImage.
