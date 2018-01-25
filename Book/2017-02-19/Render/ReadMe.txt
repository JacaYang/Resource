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

fLambert(l,v) =cdiffπ


Bibliography
[1]
Ashikhmin, Michael, Simon Premoˇze, and Peter Shirley, “A Microfacet-Based BRDF Generator,”
Computer Graphics (SIGGRAPH 2000 Proceedings)
, pp. 67–74, July 2000.
http://www.cs.utah.edu/
~shirley/papers/facets.pdf
Cited on p.
13
[2]
Ashikhmin, Michael, and Peter Shirley, “An Anisotropic Phong Light Reflection Model,” Technical Re-
port UUCS-00-014, Computer Science Department, University of Utah, June 2000.
www.cs.utah.edu/
research/techreports/2000/pdf/UUCS-00-014.pdf
Cited on p.
15, 16, 17
[3]
Ashikhmin, Michael, Simon Premoˇze, and Peter Shirley, “An Anisotropic Phong BRDF Model,”
journal
of graphics tools
, vol. 5, no. 2, pp. 25–32, 2000.
www.cs.utah.edu/~shirley/papers/jgtbrdf.pdf
Cited
on p.
15, 16, 17
[4]
Barzel, Ronen, “Lighting Controls for Computer Cinematography”
journal of graphics tools
, vol. 2, no. 1,
pp. 1–20, 1997.
Cited on p.
17
[5]
Chen, Hao, “Lighting and Material of Halo 3,”
Game Developers Conference
, March 2008.
http://www.
bungie.net/images/Inside/publications/presentations/lighting_material.zip
Cited on p.
19
[6]
Colbert, Mark, Simon Premoˇze, and Guillaume Fran ?cois, “Importance Sampling for Production Render-
ing,”
SIGGRAPH 2010 Course Notes
, 2010.
http://sites.google.com/site/isrendering/
Cited on
p.
19
[7]
Cook, Robert L., and Kenneth E. Torrance, “A Reflectance Model for Computer Graphics,”
Computer
Graphics (SIGGRAPH ’81 Proceedings)
, pp. 307–316, July 1981.
Cited on p.
16, 19
[8]
Cook, Robert L., and Kenneth E. Torrance, “A Reflectance Model for Computer Graphics,”
ACM Trans-
actions on Graphics
, vol. 1, no. 1, pp. 7–24, January 1982.
http://graphics.pixar.com/library/
ReflectanceModel/
Cited on p.
16, 19
[9]
Dorsey, Julie, Holly Rushmeier, and Fran ?cois Sillion,
Digital Modeling of Material Appearance
, Morgan
Kaufmann, 2007.
Cited on p.
19
[10]
Dutr ?e, Philip,
Global Illumination Compendium
, 1999.
http://www.graphics.cornell.edu/~phil/GI
Cited on p.
9, 19
[11]
Dutr ?e, Philip, Kavita Bala, and Philippe Bekaert,
Advanced Global Illumination
, second edition, A K
Peters Ltd., 2006.
Cited on p.
17
[12]
Glassner, Andrew S.,
Principles of Digital Image Synthesis
, vol. 1, Morgan Kaufmann, 1995.
Cited on p.
19
[13]
Glassner, Andrew S.,
Principles of Digital Image Synthesis
, vol. 2, Morgan Kaufmann, 1995.
Cited on p.
19
[14]
Gritz, Larry, and Eugene d’Eon, “The Importance of Being Linear,” in Hubert Nguyen, ed.,
GPU Gems
3
, Addison-Wesley, pp. 529–542, 2007.
http://http.developer.nvidia.com/GPUGems3/gpugems3_ch24.
html
Cited on p.
14
[15]
Hoffman, Naty, “Adventures with Gamma-Correct Rendering,” Renderwonk blog.
http://renderwonk.
com/blog/index.php/archive/adventures-with-gamma-correct-rendering/
Cited on p.
14
[16]
Kajiya, James T., “The Rendering Equation,”
Computer Graphics (SIGGRAPH ’86 Proceedings)
, pp.
143–150, August 1986.
http://www.cs.brown.edu/courses/cs224/papers/kajiya.pdf
Cited on p.
11
20
BIBLIOGRAPHY
21
[17]
Kelemen, Csaba, and L ?azl ?o Szirmay-Kalos, “A Microfacet Based Coupled Specular-Matte BRDF Model
with Importance Sampling,”
Eurographics 2001
, short presentation, pp. 25–34, September 2001.
http:
//www.fsz.bme.hu/~szirmay/scook_link.htm
Cited on p.
16, 17
[18]
Kˇriv ?anek, Jaroslav, Marcos Fajardo, Per H. Christensen, Eric Tabellion, Michael Bunnell, David Larsson,
and Anton Kaplanyan, “Global Illumination Across Industries,”
SIGGRAPH 2010 Course Notes
, 2010.
http://www.graphics.cornell.edu/~jaroslav/gicourse2010/
Cited on p.
17
[19]
Kurt, Murat, L ?aszl ?o Szirmay-Kalos, and Jaroslav Kˇriv ?anek, “An Anisotropic BRDF Model for Fitting
and Monte Carlo Rendering,”
Computer Graphics
, vol. 44, no. 1, pp. 1–15, 2010.
http://www.graphics.
cornell.edu/~jaroslav/
Cited on p.
15, 16
[20]
Akenine-M ?oller, Tomas, Eric Haines, and Naty Hoffman,
Real-Time Rendering
, third edition, A K Peters
Ltd., 2008.
http://realtimerendering.com/
Cited on p.
9, 19
[21]
Oren, Michael, and Shree K. Nayar, “Generalization of Lambert’s Reflectance Model,”
Computer Graphics
(SIGGRAPH 94 Proceedings)
, pp. 239–246, July 1994.
http://www.cs.columbia.edu/CAVE/projects/
oren/
Cited on p.
17
[22]
Schlick, Christophe, “An Inexpensive BDRF Model for Physically based Rendering,”
Computer Graphics
Forum
, vol. 13, no. 3, Sept. 1994, pp. 149–162.
http://dept-info.labri.u-bordeaux.fr/~schlick/
DOC/eur2.html
Cited on p.
14
[23]
Sch ?uler, Christian, “An Efficient and Physically Plausible Real Time Shading Model,” in Wolfgang Engel,
ed.,
ShaderX
7
, Charles River Media, pp. 175–187, 2009.
Cited on p.
19
[24]
Shirley, Peter, Helen Hu, Brian Smits, Eric Lafortune, “A Practitioners’ Assessment of Light Reflec-
tion Models,”
Pacific Graphics ’97
, pp. 40–49, October 1997.
http://www.graphics.cornell.edu/pubs/
1997/SHSL97.html
Cited on p.
17
[25]
Walter, Bruce, Stephen R. Marschner, Hongsong Li, Kenneth E. Torrance, “Microfacet Models for Re-
fraction through Rough Surfaces,”
Eurographics Symposium on Rendering (2007)
, 195–206, June 2007.
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.html
Cited on p.
10, 13, 15, 16
[26]
Ward, Gregory, “Measuring and Modeling Anisotropic Reflection,”
Computer Graphics (SIGGRAPH ’92
Proceedings)
, pp. 265–272, July 1992.
http://radsite.lbl.gov/radiance/papers/sg92/paper.html
Cited on p.
15

















