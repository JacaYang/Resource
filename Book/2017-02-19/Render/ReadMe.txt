ReadMe

===============
Instant Radiosity
Alexander Keller
Universit at Kaiserslautern
https://www.cg.tuwien.ac.at/courses/RendEng/RendEng-2016-01-11-InstantRadiosity.pdf

================
The Irradiance Volume
Gene Greger , Peter Shirley, Philip M. Hubbard, Donald P. Greenberg
Program of Computer Graphics
580 Rhodes Hall
Cornell University 
Ithaca, NY 14853
http://www.cs.utah.edu/~shirley/papers/irradiance.pdf

=================
Irradiance Volumes for Games
Natalya Tatarchuk
3D Application Research Group
ATI Research, Inc.
http://developer.amd.com/wordpress/media/2012/10/Tatarchuk_Irradiance_Volumes.pdf

==============
游戏中的Irradiance Volume
http://blog.csdn.net/toughbro/article/details/53026729

reference

The Irradiance Volume
Irradiance Volumes for Games
Shading in Valve’s Source Engine
DeferredRadianceTransfer
Volumetric Global Illumination At Treyarch
Siggraph2009_BlackRock



http://gdcvault.com/play/1015326/Deferred-Radiance-Transfer-Volumes-Global


Chapter 8 
Shading in Valve’s Source Engine 
http://www.valvesoftware.com/publications/2006/SIGGRAPH06_Course_ShadingInValvesSourceEngine.pdf


Irradiance Volumes for Games
Natalya Tatarchuk
3D Application Research Group
ATI Research, Inc.
http://developer.amd.com/wordpress/media/2012/10/Tatarchuk_Irradiance_Volumes.pdf



The Irradiance Volume
https://pdfs.semanticscholar.org/40cb/9a27cfd69a5c5c891741ce02961d2d76c639.pdf?_ga=1.233735774.1506007508.1478184009

=================
东拼西凑PBR：PBR基础.pdf

https://www.allegorithmic.com/system/files/software/download/build/PBR_Guide_Vol.1.pdf

f (l,v) = fLambert (l,v)(1? Fmacro (v,n))+ fCook?Torrance (l,v)

http://renderwonk.com/publications/s2010-shading-course/hoffman/s2010_physically_based_shading_hoffman_a_notes.pdf

==================
https://www.allegorithmic.com/system/files/software/download/build/PBR_Guide_Vol.1.pdf

F0 (Fresnel Reflectance at 0 Degrees)

The BRDF used by Substance's PBR shaders is based on
Disney's "principled" reflectance model, which is based on
the GGX microfacet distribution. GGX provides one of the
better solutions in terms of specular distribution in that it
has a shorter peak in the highlight and a longer tail in the
falloff, which is to say that it looks
more realistic as shown in figure 08.

References
1. Physically-Based Shading at Disney Brent Burley, Walt Disney Animation Studios.
https://disney-animation.s3.amazonaws.com/library/s2012_pbs_disney_brdf_notes_v2.pdf
2. Microfacet Models for Refraction through Rough Surfaces
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.pdf
3. Feeding a Physically-Based Shading Model by Sebastien Lagarde
http://seblagarde.wordpress.com/2011/08/17/feeding-a-physical-based-lighting-mode/
4. An Introduction to BRDF Models by Dani?l Jimenez Kwast
http://hmi.ewi.utwente.nl/verslagen/capita-selecta/CS-Jimenez-Kwast-Daniel.pdf

=============================
http://renderwonk.com/publications/s2010-shading-course/hoffman/s2010_physically_based_shading_hoffman_a_notes.pdf

cspeclooks like an ideal parameter for a Fresnel reflectance approximation, and indeed Schlick [22]gives a cheap and reasonably accurate approximation that uses it:FSchlick(cspec,l,n) =cspec+ (1?cspec)(1?(l·n))5(5)This approximation is widely used in computer graphics. In the special case of active microfacets,hmust be substituted for the surface normaln:FSchlick(cspec,l,h) =cspec+ (1?cspec)(1?(l·h))5(6)





















