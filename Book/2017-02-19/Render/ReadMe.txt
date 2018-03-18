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
ÓÎÏ·ÖÐµÄIrradiance Volume
http://blog.csdn.net/toughbro/article/details/53026729

reference

The Irradiance Volume
Irradiance Volumes for Games
Shading in Valve¡¯s Source Engine
DeferredRadianceTransfer
Volumetric Global Illumination At Treyarch
Siggraph2009_BlackRock



http://gdcvault.com/play/1015326/Deferred-Radiance-Transfer-Volumes-Global


Chapter 8 
Shading in Valve¡¯s Source Engine 
http://www.valvesoftware.com/publications/2006/SIGGRAPH06_Course_ShadingInValvesSourceEngine.pdf


Irradiance Volumes for Games
Natalya Tatarchuk
3D Application Research Group
ATI Research, Inc.
http://developer.amd.com/wordpress/media/2012/10/Tatarchuk_Irradiance_Volumes.pdf



The Irradiance Volume
https://pdfs.semanticscholar.org/40cb/9a27cfd69a5c5c891741ce02961d2d76c639.pdf?_ga=1.233735774.1506007508.1478184009

=================
¶«Æ´Î÷´ÕPBR£ºPBR»ù´¡.pdf

https://www.allegorithmic.com/system/files/software/download/build/PBR_Guide_Vol.1.pdf

f (l,v) = fLambert (l,v)(1? Fmacro (v,n))+ fCook?Torrance (l,v)

http://renderwonk.com/publications/s2010-shading-course/hoffman/s2010_physically_based_shading_hoffman_a_notes.pdf

==================
?½ð½ðÊô?¸ß¹â¿ÉÄÜÓÐÑÕ?É«£¨F0ÓÐÑÕ?É«£©£¬?·Ç?½ð½ðÊô?¸ß¹â?ÎÞÑÕ?É«£¨F0Îª»Ò¶È

https://www.allegorithmic.com/system/files/software/download/build/PBR_Guide_Vol.1.pdf

page 9
It is the F0 reflectance value that we
are concerned with in regards to
authoring our textures. Non-metals
(dielectrics/insulators) will have a
greyscale value and metals (conductors)
will have an RGB value.

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

cspeclooks like an ideal parameter for a Fresnel reflectance approximation, and indeed Schlick [22]gives a cheap and reasonably accurate approximation that uses it:FSchlick(cspec,l,n) =cspec+ (1?cspec)(1?(l¡¤n))5(5)This approximation is widely used in computer graphics. In the special case of active microfacets,hmust be substituted for the surface normaln:FSchlick(cspec,l,h) =cspec+ (1?cspec)(1?(l¡¤h))5(6)

fLambert(l,v) =cdiff¦Ð


Bibliography
[1]
Ashikhmin, Michael, Simon Premo¡¦ze, and Peter Shirley, ¡°A Microfacet-Based BRDF Generator,¡±
Computer Graphics (SIGGRAPH 2000 Proceedings)
, pp. 67¨C74, July 2000.
http://www.cs.utah.edu/
~shirley/papers/facets.pdf
Cited on p.
13
[2]
Ashikhmin, Michael, and Peter Shirley, ¡°An Anisotropic Phong Light Reflection Model,¡± Technical Re-
port UUCS-00-014, Computer Science Department, University of Utah, June 2000.
www.cs.utah.edu/
research/techreports/2000/pdf/UUCS-00-014.pdf
Cited on p.
15, 16, 17
[3]
Ashikhmin, Michael, Simon Premo¡¦ze, and Peter Shirley, ¡°An Anisotropic Phong BRDF Model,¡±
journal
of graphics tools
, vol. 5, no. 2, pp. 25¨C32, 2000.
www.cs.utah.edu/~shirley/papers/jgtbrdf.pdf
Cited
on p.
15, 16, 17
[4]
Barzel, Ronen, ¡°Lighting Controls for Computer Cinematography¡±
journal of graphics tools
, vol. 2, no. 1,
pp. 1¨C20, 1997.
Cited on p.
17
[5]
Chen, Hao, ¡°Lighting and Material of Halo 3,¡±
Game Developers Conference
, March 2008.
http://www.
bungie.net/images/Inside/publications/presentations/lighting_material.zip
Cited on p.
19
[6]
Colbert, Mark, Simon Premo¡¦ze, and Guillaume Fran ?cois, ¡°Importance Sampling for Production Render-
ing,¡±
SIGGRAPH 2010 Course Notes
, 2010.
http://sites.google.com/site/isrendering/
Cited on
p.
19
[7]
Cook, Robert L., and Kenneth E. Torrance, ¡°A Reflectance Model for Computer Graphics,¡±
Computer
Graphics (SIGGRAPH ¡¯81 Proceedings)
, pp. 307¨C316, July 1981.
Cited on p.
16, 19
[8]
Cook, Robert L., and Kenneth E. Torrance, ¡°A Reflectance Model for Computer Graphics,¡±
ACM Trans-
actions on Graphics
, vol. 1, no. 1, pp. 7¨C24, January 1982.
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
Gritz, Larry, and Eugene d¡¯Eon, ¡°The Importance of Being Linear,¡± in Hubert Nguyen, ed.,
GPU Gems
3
, Addison-Wesley, pp. 529¨C542, 2007.
http://http.developer.nvidia.com/GPUGems3/gpugems3_ch24.
html
Cited on p.
14
[15]
Hoffman, Naty, ¡°Adventures with Gamma-Correct Rendering,¡± Renderwonk blog.
http://renderwonk.
com/blog/index.php/archive/adventures-with-gamma-correct-rendering/
Cited on p.
14
[16]
Kajiya, James T., ¡°The Rendering Equation,¡±
Computer Graphics (SIGGRAPH ¡¯86 Proceedings)
, pp.
143¨C150, August 1986.
http://www.cs.brown.edu/courses/cs224/papers/kajiya.pdf
Cited on p.
11
20
BIBLIOGRAPHY
21
[17]
Kelemen, Csaba, and L ?azl ?o Szirmay-Kalos, ¡°A Microfacet Based Coupled Specular-Matte BRDF Model
with Importance Sampling,¡±
Eurographics 2001
, short presentation, pp. 25¨C34, September 2001.
http:
//www.fsz.bme.hu/~szirmay/scook_link.htm
Cited on p.
16, 17
[18]
K¡¦riv ?anek, Jaroslav, Marcos Fajardo, Per H. Christensen, Eric Tabellion, Michael Bunnell, David Larsson,
and Anton Kaplanyan, ¡°Global Illumination Across Industries,¡±
SIGGRAPH 2010 Course Notes
, 2010.
http://www.graphics.cornell.edu/~jaroslav/gicourse2010/
Cited on p.
17
[19]
Kurt, Murat, L ?aszl ?o Szirmay-Kalos, and Jaroslav K¡¦riv ?anek, ¡°An Anisotropic BRDF Model for Fitting
and Monte Carlo Rendering,¡±
Computer Graphics
, vol. 44, no. 1, pp. 1¨C15, 2010.
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
Oren, Michael, and Shree K. Nayar, ¡°Generalization of Lambert¡¯s Reflectance Model,¡±
Computer Graphics
(SIGGRAPH 94 Proceedings)
, pp. 239¨C246, July 1994.
http://www.cs.columbia.edu/CAVE/projects/
oren/
Cited on p.
17
[22]
Schlick, Christophe, ¡°An Inexpensive BDRF Model for Physically based Rendering,¡±
Computer Graphics
Forum
, vol. 13, no. 3, Sept. 1994, pp. 149¨C162.
http://dept-info.labri.u-bordeaux.fr/~schlick/
DOC/eur2.html
Cited on p.
14
[23]
Sch ?uler, Christian, ¡°An Efficient and Physically Plausible Real Time Shading Model,¡± in Wolfgang Engel,
ed.,
ShaderX
7
, Charles River Media, pp. 175¨C187, 2009.
Cited on p.
19
[24]
Shirley, Peter, Helen Hu, Brian Smits, Eric Lafortune, ¡°A Practitioners¡¯ Assessment of Light Reflec-
tion Models,¡±
Pacific Graphics ¡¯97
, pp. 40¨C49, October 1997.
http://www.graphics.cornell.edu/pubs/
1997/SHSL97.html
Cited on p.
17
[25]
Walter, Bruce, Stephen R. Marschner, Hongsong Li, Kenneth E. Torrance, ¡°Microfacet Models for Re-
fraction through Rough Surfaces,¡±
Eurographics Symposium on Rendering (2007)
, 195¨C206, June 2007.
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.html
Cited on p.
10, 13, 15, 16
[26]
Ward, Gregory, ¡°Measuring and Modeling Anisotropic Reflection,¡±
Computer Graphics (SIGGRAPH ¡¯92
Proceedings)
, pp. 265¨C272, July 1992.
http://radsite.lbl.gov/radiance/papers/sg92/paper.html
Cited on p.
15

=================
https://disney-animation.s3.amazonaws.com/library/s2012_pbs_disney_brdf_notes_v2.pdf

metallic - the metallic-ness (0 = dielectric, 1 = metallic). This is a linear blend between two
dierent models. The metallic model has no diuse component and also has a tinted incident
specular, equal to the base color.


5.3 Diuse model details
Some models include a diuse Fresnel factor such as:
(1 ?? F(l))(1 ?? F(d))


DGTR2(h) = 2

1
(1 + (2 ?? 1) cos2 h)2



FSchlick = F0 + (1 ?? F0)(1 ?? cos d)5
The constant, F0, represents the specular re
ectance at normal incidence and is achromatic for
dielectrics and chromatic (i.e. tinted) for metals. The actual value depends on the index of refraction.
Note that specular re
ection comes from microfacets and thus F depends on d, the angle between
the light vector and the micronormal (i.e. the half-vector), not the angle of incidence with the surface
normal.



References
[1] Michael Ashikhmin. Distribution-based brdfs. Technical report, 2007.
[2] Michael Ashikhmin, Simon Premoze, and Peter Shirley. A Microfacet-Based BRDF generator. In
Sheila Homeyer, editor, Proceedings of the Computer Graphics Conference 2000 (SIGGRAPH-
00), pages 65{74, New York, July 23{28 2000. ACMPress.
[3] Michael Ashikhmin and Peter Shirley. An anisotropic Phong BRDF model. Journal of Graphics
Tools: JGT, 5(2):25{32, 2000.
[4] M. M. Bagher, C. Soler, and N. Holzschuch. Accurate tting of measured re
ectances using a
shifted gamma micro-facet distribution. Computer Graphics Forum, 31(4):1509{1518, 2012.
19
[5] P. Beckmann and A. Spizzichino. The scattering of electromagnetic waves from rough surfaces.
MacMillan, 1963.
[6] James F. Blinn. Models of light re
ection for computer synthesized pictures. volume 11, pages
192{198, July 1977.
[7] R. L. Cook and K. E. Torrance. A re
ectance model for computer graphics. Computer Graphics,
15(3):307{316, 1981.
[8] Arne Dur. An improved normalization for the Ward re
ectance model. Journal of graphics, gpu,
and game tools, 11(1):51{59, 2006.
[9] Dave Edwards, Solomon Boulos, Jared Johnson, Peter Shirley, Michael Ashikhmin, Michael Stark,
and Chris Wyman. The halfway vector disk for brdf modeling. ACM Trans. Graph., 25(1):1{18,
January 2006.
[10] David Geisler-Moroder and Arne Dur. A new Ward BRDF model with bounded albedo. Comput.
Graph. Forum, 29(4):1391{1398, 2010.
[11] Pat Hanrahan and Wolfgang Krueger. Re
ection from layered surfaces due to subsurface scattering.
In Proceedings of the 20th annual conference on Computer graphics and interactive techniques,
SIGGRAPH '93, pages 165{174, New York, NY, USA, 1993. ACM.
[12] Xiao D. He, Kenneth E. Torrance, Francois X. Sillion, and Donald P. Greenberg. A Comprehensive
Physical Model for Light Re
ection. In Computer Graphics (ACM SIGGRAPH '91 Proceedings),
volume 25, pages 175{186, July 1991.
[13] Csaba Kelemen, Laszlo Szirmay-Kalos, and Laszlo Szirmay-kalos. A microfacet based coupled
specular-matte brdf model with importance sampling. Eurographics Short Presentations, 2001.
[14] Murat Kurt, Laszlo Szirmay-Kalos, and Jaroslav Krivanek. An anisotropic brdf model for tting
and monte carlo rendering. SIGGRAPH Comput. Graph., 44(1):3:1{3:15, February 2010.
[15] Eric P. Lafortune, Sing-Choong Foo, Kenneth E. Torrance, and Donald P. Greenberg. Nonlinear
approximation of re
ectance functions. In Computer Graphics (ACM SIGGRAPH '97
Proceedings), volume 31, pages 117{126, 1997.
[16] Robert R. Lewis. Making Shaders More Physically Plausible. In Fourth Eurographics Workshop
on Rendering, number Series EG 93 RW, pages 47{62, Paris, France, June 1993.
[17] Joakim Low, Joel Kronander, Anders Ynnerman, and Jonas Unger. Brdf models for accurate and
ecient rendering of glossy surfaces. ACM Trans. Graph., 31(1):9:1{9:14, February 2012.
[18] Wojciech Matusik, Hanspeter Pster, Matt Brand, and Leonard McMillan. A data-driven re-

ectance model. ACM Transactions on Graphics, 22(3):759{769, July 2003.
[19] Laszlo Neumann, Attila Neumann, and Laszlo Szirmay-Kalos. Compact metallic re
ectance models.
Computer Graphics Forum, 18(3):161{172, September 1999. ISSN 1067-7055.
[20] Laszlo Neumann, Attila Neumann, and Laszlo Szirmay-Kalos. Re
ectance models by pumping
up the albedo function. In Machine Graphics and Vision, pages 3{18, 1999.
[21] Addy Ngan, Fredo Durand, and Wojciech Matusik. Experimental analysis of BRDF models. In
Kavita Bala and Philip Dutre, editors, Eurographics Symposium on Rendering, pages 117{126,
Konstanz, Germany, 2005. Eurographics Association.
20
[22] Ko Nishino and Stephen Lombardi. Directional statistics-based re
ectance model for isotropic
bidirectional re
ectance distribution functions. J. Opt. Soc. Am. A, 28(1):8{18, Jan 2011.
[23] Michael Oren and Shree K. Nayar. Generalization of lambert's re
ectance model. In SIGGRAPH,
pages 239{246. ACM, 1994.
[24] Romain Pacanowski, Oliver Salazar Celis, Christophe Schlick, Xavier Granier, Pierre Poulin,
and Annie Cuyt. Rational brdf. IEEE Transactions on Visualization and Computer Graphics,
99(PrePrints), 2012.
[25] Bui-T. Phong. Illumination for computer generated pictures. Communications of the ACM,
18(6):311{317, June 1975.
[26] Fabiano Romeiro, Yuriy Vasilyev, and Todd Zickler. Passive re
ectometry. In Proceedings of
the 10th European Conference on Computer Vision: Part IV, ECCV '08, pages 859{872, Berlin,
Heidelberg, 2008. Springer-Verlag.
[27] Iman Sadeghi, Heather Pritchett, Henrik Wann Jensen, and Rasmus Tamstorf. An artist friendly
hair shading system. In ACM SIGGRAPH 2010 papers, SIGGRAPH '10, pages 56:1{56:10, New
York, NY, USA, 2010. ACM.
[28] Christophe Schlick. An Inexpensive BRDF Model for Physically-Based Rendering. Computer
Graphics Forum, 13(3):233{246, 1994.
[29] B. Smith. Geometrical shadowing of a random rough surface. IEEE Trans. Ant. and Propagation,
AP-15(5):668{671, September 1967.
[30] K. Torrance and E. Sparrow. Theory for o-specular re
ection from roughened surfaces. J. Optical
Soc. America, 57:1105{1114, 1967.
[31] S. Trowbridge and K. P. Reitz. Average irregularity representation of a rough ray re
ection.
Journal of the Optical Society of America, 65(5):531{536, May 1975.
[32] Bruce Walter. Notes on the Ward BRDF. Technical Report PCG-05-06, Cornell Program of
Computer Graphics, 2005.
[33] Bruce Walter, Stephen R. Marschner, Hongsong Li, and Kenneth E. Torrance. Microfacet models
for refraction through rough surfaces. In Proceedings of the Eurographics Symposium on Rendering,
2007.
[34] Gregory J. Ward. Measuring and modeling anisotropic re
ection. In Edwin E. Catmull, editor,
Computer Graphics (SIGGRAPH '92 Proceedings), volume 26, pages 265{272, July 1992.
[35] L. B. Wol, S. K. Nayar, and M. Oren. Improved diuse re
ection models for computer vision.
International Journal of Computer Vision, 30(1):55{71, October 1998.
A Selected history of BRDF models used in graphics
 Beckmann 1963 [5] provided a model for scattering from rough surfaces based on a Gaussian
distribution of surface slopes.
 Torrance and Sparrow 1967 [30] introduced the microfacet model. A Gaussian distribution of
microfacet angles was assumed and a microfacet shadowing factor was derived from simplied
geometric assumptions.
21
 Smith 1967 [29] derived a shadowing function from the microfacet distribution. Notably, this
shadowing function varied with surface roughness.
 Phong 1975 [25] proposed a computationally simple model of a specular highlight using an exponentiated
cosine.
 Trowbridge and Reitz 1975 [31] derived a new microfacet distribution based on average surface
irregularity of curved microsurfaces derived from an ellipsoid of revolution. They t their model
to measured data for rough glass and compared their results with Gaussian, Beckmann, Sirohi,
and Berry distributions.
 Blinn 1977 [6] implemented the Torrance-Sparrow model with the Trowbridge-Reitz distribution
(chosen for its computational eciency as well as its physical basis). Blinn also proposed a
microfacet distribution based based on the Phong model, commonly referred to as \Blinn Phong,"
by adapting it to the more physically-correct half-vector formulation.
 Cook and Torrance 1981 [7] implemented the Torrance-Sparrow model with the Beckmann distribution
and studied spectral shifts due to the Fresnel factor.
 He, Torrance, Sillion, and Greenberg 1991 [12] presented a model that included specular, directional
diuse, and uniform diuse components. The model is derived for polarized light and
simplied for unpolarized light.
 Ward 1992 [34] presented an anisotropic specular model derived from the Beckmann distribution.
Walter 2005 [32] provided a more ecient exact implementation.
 Lewis 1993 [16] proposed a \modied Phong" model that included a normalization term for
energy conservation.
 Hanrahan and Krueger 1993 [11] developed a diuse BRDF model that approximates subsurface
transport.
 Oren and Nayar 1994 [23] derived a diuse model for rough surfaces based on Lambertian microfacets.
 Schlick 1994 [28] developed rational approximations to the various components of the microfacet
model. The Schlick Fresnel approximation is widely used. Also, Schlick recognized the discontinuity
in the Torrance-Sparrow shadowing term and suggested an approximation of the Smith
shadowing function as an alternative. Schlick also presented an approximation to the Beckmann
distribution.
 Lafortune 1997 [15] proposed using a sum of arbitrarily-oriented Phong lobes as the basis for a
general model.
 Wol, Nayar and Oren 1998 [35] developed an improved diuse model for very smooth surfaces
which are darker at grazing angles than Lambert diuse due to the Fresnel eect. This model is
also combined in an approximate form with the Oren Nayar model to represent a continuum of
smooth to rough diuse surfaces.
 Neumann et al. 1999 [19] proposed a \stretched Phong" model intended for metallic surfaces
that has an albedo that becomes 
at as the surface becomes shiny.
22
 Neumann et al. 1999b [20] proposed a process to \pump up" the albedo of arbitrary BRDFs to
improve energy balance. Previous models were shown to have an albedo that falls o too quickly
with incident angle (except for the Ward model which is shown to diverge at grazing incidence).
Each iterative pump-up divides the BRDF by a measured correction factor making the albedo
progressively 
atter.
 Ashikhmin, Premoze, and Shirley 2000 [2] derived a shadowing function from numeric integration
of arbitrary microfacet distributions.
 Ashikhmin and Shirley 2000 [3] presented a anisotropic Phong model that included a Fresnelweighted
diuse and energy conservation guarantees.
 Kelemen and Szirmay-Kalos 2001 [13] proposed an alternative shadowing term that approximates
the Torrance-Sparrow shadowing function with a dierentiable form. A coupled-diuse model is
also proposed such that the total albedo is always 1.
 Dur 2006 [8] improved the energy balance of the Ward model.
 Edwards et al. 2006 [9] proposed the \halfway vector disk" as a new domain for modeling
specular distributions with the goal of perfect energy conservation (albedo = 1). An alternate
non-conservative form is also presented for data tting.
 Ashikhmin and Premoze 2007 [1] presented the \distribution BRDF" which smooths out the
discontinuity in the shadowing term of Ashikhmin Shirley. A simple method for estimating
specular distributions from backscattering images (such as from a single 
ash-lit photograph) is
also provided.
 Walter et al. 2007 [33] derived Smith shadowing functions for the Phong and GGX distributions
and provided an approximation of Smith shadowing for the Beckmann distribution. Note: GGX
is equivalent to the Trowbridge-Reitz distribution.
 Romeiro et al. 2008 [26] showed than the MERL materials are well-represented by a simple
bivariate form, (h; thetad) and exploited this fact to proposed a simplied BRDF capture
method.
 Geisler-Moroder and Dur 2010 [10] further rened this model to restore Helmholtz reciprocity
and guarantee energy conservation.
 Kurt et al 2010 [14] extended the Beckmann distribution to anisotropic form and proposed a
new parameterized shadowing function giving control over albedo and improving tting for some
materials. Two specular lobes are suggested for tting many of the MERL materials.
 Nishino and Lombardi 2011 [22] proposed the \hemispherical exponential power distribution" or
\Hemi-EPD" which has an additional degree of freedom to improve tting power. The Hemi-
EPD is used as a basis for the entire BRDF and parameters are t to individual d slices and
interpolated. Additionally, multiple lobes per d slice are required for many materials.
 Low et al. 2012 [17] proposed a new \ABC" microfacet distribution inspired by Rayleigh-Rice
smooth-surface scattering theory. Additionally, the \projected deviation vector" is presented as
an alternative to the half-vector parameterization for data tting.
 Pacanowski et al. 2012 [24] developed a framework for tting rational functions to general
isotropic BRDFs over the (h; d) domain. An anisotropic form is also proposed as a simple
scaling of the isotropic form with respect to h.
23
 Bagher et al. 2012 [4] proposed a new \shifted gamma" or \SGD" microfacet distribution derived
to t the range of observed slopes in the MERL database. An approximation of the Smith
shadowing function for the SGD distribution is provided. Additionally, the Fresnel term is
modied with a correction term providing an additional degree of freedom, improving tting
ability.

================
¸ß¹âBRDF»¯¼ò¹«Ê½
http://blog.csdn.net/xuexiaokkk/article/details/48489289

References
[1] Hoffman 2013, "Background: Physics and Math of Shading"
[2] Blinn 1977, "Models of light reflection for computer synthesized pictures"
[3] Beckmann 1963, "The scattering of electromagnetic waves from rough surfaces"
[4] Walter et al. 2007, "Microfacet models for refraction through rough surfaces"
[5] Burley 2012, "Physically-Based Shading at Disney"
[6] Neumann et al. 1999, "Compact metallic reflectance models"
[7] Kelemen 2001, "A microfacet based coupled specular-matte brdf model with importance sampling"
[8] Smith 1967, "Geometrical shadowing of a random rough surface"
[9] Schlick 1994, "An Inexpensive BRDF Model for Physically-Based Rendering"
[10] Karis 2013, "Real Shading in Unreal Engine 4"
[11] Cook and Torrance 1982, "A Reflectance Model for Computer Graphics"
[12] Reed 2013, "How Is the NDF Really Defined?"

=====================
Unity5 GIÓëPBSäÖÈ¾´ÓÓÃ·¨µ½×ÅÉ«´úÂë
https://www.cnblogs.com/zhouxin/p/5168632.html
 
======================
»ùÓÚÎïÀíµÄäÖÈ¾¡ª¸ü¾«È·µÄÎ¢±íÃæ·Ö²¼º¯ÊýGGX
https://blog.uwa4d.com/archives/1582.html
ÏÂÔØÁ´½Ó£º
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.html

²Î¿¼ÎÄÏ×£º
¡¾1¡¿ P.Beckmann and A. Spizzichino, The Scattering of Electromagnetic Waves from Rough Surfaces, Pergamon Press, New York 1963.
¡¾2¡¿ http://blog.selfshadow.com/publications/s2013-shading-course/karis/s2013_pbs_epic_notes_v2.pdf
¡¾3¡¿ K.E.Torrance, E. M. Sparrow : Theory for off-specular reflection from roughened surfaces. Journal of Optical Society of America 57, 9(1967), 1105¨C1114.
¡¾4¡¿ https://blogs.unity3d.com/cn/2016/01/25/ggx-in-unity-5-3/

ÕâÊÇÙ§»¢¿Æ¼¼µÚ203ÆªÔ­´´ÎÄÕÂ£¬»¶Ó­×ª·¢·ÖÏí£¬Î´¾­×÷ÕßÊÚÈ¨ÇëÎð×ªÔØ¡£Èç¹ûÄúÒ²ÓÐÈÎºÎ¶Àµ½µÄ¼û½â»òÕßÈ«ÐÂµÄ·¢ÏÖÒ²»¶Ó­ÁªÏµÎÒÃÇ£¬Ò»ÆðÌ½ÌÖ¡££¨QQÈº465082844£©
============================
»ùÓÚÎïÀí×ÅÉ«(PBS)¼°UnityÖÐµÄÊµÏÖ
http://blog.csdn.net/liumazi/article/details/72927529
È«¾Ö¹âÕÕ¼¼Êõ£º´ÓÀëÏßµ½ÊµÊ±äÖÈ¾     http://www.thegibook.com/

Unity Shader ÈëÃÅ¾«Òª     https://github.com/candycat1992/Unity_Shaders_Book

»ùÓÚÎïÀí×ÅÉ«ÏµÁÐ     https://zhuanlan.zhihu.com/p/20091064

»ùÓÚÎïÀíµÄBRDF     http://www.klayge.org/wiki/index.php/%E5%9F%BA%E4%BA%8E%E7%89%A9%E7%90%86%E7%9A%84BRDF

»ùÓÚÎïÀíµÄäÖÈ¾¡ªµÏÊ¿ÄáµÄäÖÈ¾Ä£ÐÍ     https://zhuanlan.zhihu.com/p/25427105
=====================
¸ß¹âBRDF»¯¼ò¹«Ê½×Ü½á£¨×ª£©
http://blog.csdn.net/aidlife/article/details/46792177
References
[1] Hoffman 2013, "Background: Physics and Math of Shading"
[2] Blinn 1977, "Models of light reflection for computer synthesized pictures"
[3] Beckmann 1963, "The scattering of electromagnetic waves from rough surfaces"
[4] Walter et al. 2007, "Microfacet models for refraction through rough surfaces"
[5] Burley 2012, "Physically-Based Shading at Disney"
[6] Neumann et al. 1999, "Compact metallic reflectance models"
[7] Kelemen 2001, "A microfacet based coupled specular-matte brdf model with importance sampling"
[8] Smith 1967, "Geometrical shadowing of a random rough surface"
[9] Schlick 1994, "An Inexpensive BRDF Model for Physically-Based Rendering"
[10] Karis 2013, "Real Shading in Unreal Engine 4"
[11] Cook and Torrance 1982, "A Reflectance Model for Computer Graphics"
[12] Reed 2013, "How Is the NDF Really Defined?"

==============
¸ß¹âBRDF»¯¼ò¹«Ê½
http://blog.csdn.net/xuexiaokkk/article/details/48489289

[5] Burley 2012, "Physically-Based Shading at Disney"
http://blog.selfshadow.com/publications/s2012-shading-course/

=================
http://blog.selfshadow.com/publications/s2012-shading-course/

11:15 Physically Based Shading at Disney (Brent Burley) [slides: keynote, pdf] [course notes]

================
http://blog.selfshadow.com/publications/s2012-shading-course/burley/s2012_pbs_disney_brdf_slides_v2.pdf

¸ß¹âBRDF»¯¼ò¹«Ê½
http://blog.csdn.net/xuexiaokkk/article/details/48489289
µã»÷
[5] Burley 2012, "Physically-Based Shading at Disney"
½øÈë
http://blog.selfshadow.com/publications/s2012-shading-course/
µã»÷
11:15 Physically Based Shading at Disney (Brent Burley) [slides: keynote, pdf] [course notes]
½øÈë
http://blog.selfshadow.com/publications/s2012-shading-course/burley/s2012_pbs_disney_brdf_slides_v2.pdf

=====================
Schlick's approximation ÊÇ·Çµ¼Ìå½üËÆ

https://en.wikipedia.org/wiki/Schlick%27s_approximation

In 3D computer graphics, Schlick's approximation, named after Christophe Schlick, is a formula for approximating the contribution of the Fresnel factor in the specular reflection of light from a non-conducting interface (surface) between two media.[1]

See also

Computer graphics portal 

Phong reflection model
Blinn-Phong shading model
Fresnel equations

References

Schlick, C. (1994). "An Inexpensive BRDF Model for Physically-based Rendering" (PDF). Computer Graphics Forum. 13 (3): 233. doi:10.1111/1467-8659.1330233.
Hoffman, Naty (2013). "Background: Physics and Math of Shading" (PDF). Fourth International Conference and Exhibition on Computer Graphics and Interactive Techniques.

===============
Âþ·´Éä·ÆÄá¶ûÏµÊý
ÕâÓ¦¸ÃÊÇ¸öÖÁ½ñÉÐÎÞ¶¨ÂÛµÄÎÊÌâ£¬°æ±¾ºÜ¶à£¬¸÷ÖÖÅä±ÈÏµÊý¶¼ÓÐÊ¹ÓÃ£¬ÎÒÑ¡ÁËÒ»¸ö×Ô¼ºÈÏÎªÓÐµÀÀíµÄ¡£
https://www.allegorithmic.com/system/files/software/download/build/PBR_Guide_Vol.1.pdf 

=============
var(¿ÖÁúµ°)(350479720) 9:40:37
º®ËªµÄÕâ¸öÆÁÄ»¿Õ¼ä·´ÉäÓÐÈË¿´¹ýÂð?
var(¿ÖÁúµ°)(350479720) 9:40:52
http://www.cse.chalmers.se/edu/year/2017/course/TDA361/Advanced%20Computer%20Graphics/Screen-space%20reflections.pdf

================
s2010_physically_based_shading_hoffman_a_notes.pdf

cspec looks like an ideal parameter for a Fresnel re¡ãectance approximation, and indeed Schlick [22]
gives a cheap and reasonably accurate approximation that uses it:
FSchlick(cspec; l; n) = cspec + (1 ? cspec)(1 ? (l ¡é n))5 (5)
This approximation is widely used in computer graphics. In the special case of active microfacets,
h must be substituted for the surface normal n:
FSchlick(cspec; l; h) = cspec + (1 ? cspec)(1 ? (l ¡é h))5 (6)
To know which values are reasonable to assign to cspec, it is instructive to look at the values of F(0¡À)
for various real-world materials. These can be found in Table 1. Values are given in both linear and
gamma (sRGB) space; we recommend anyone unfamiliar with the importance of computing shading in
linear space and the issues involved in converting input from gamma space consult some of the articles
on the topic ([14, 15]).


Although there are several models for subsurface local re¡ãection in the literature, the most widely-used
one by far is the Lambertian BRDF term. The Lambertian BRDF is actually a constant value; the
well-known cosine or (n ¡é l) factor is part of the re¡ãection equation, not the BRDF (as we saw in
Equation 1). The exact value of the Lambertian BRDF is:
fLambert(l; v) =
cdi?
?
: (7)

Practical Implementation of Physically-Based Shading Models at tri-Ace
gives a specular implementation for constant and SH ambient, a recent presentation by Bungie [5]
discusses applying the Cook-Torrance [7, 8] specular term to SH lighting, and a ShaderX7 article
by Sch?uler [23] describes an implementation of a physically-based specular term with hemispherical
lighting.

Other aspects of image-based lighting in ¡¥lm production are discussed in Ben Snow's
talk in this course, Terminators and Iron Men: Image-Based Lighting and Physical Shading at ILM,
and some aspects of shading with environment maps for video games are discussed in Naty Ho?man's
other talk, Crafting Physically Motivated Shading Models for Game Development.

===============
Ogre ¾ÍÊÇÍêÈ«²Î¿¼ÕâÀïÊµÏÖµÄ
s2013_pbs_epic_notes_v2.pdf

f(l; v) =
cdiff


Specular D
For the normal distribution function (NDF), we found Disney¡¯s choice of GGX/Trowbridge-Reitz to
be well worth the cost. The additional expense over using Blinn-Phong is fairly small, and the distinct,
natural appearance produced by the longer ¡°tail¡± appealed to our artists. We also adopted Disney¡¯s
reparameterization of  = Roughness2.
D(h) =
2
 ((n  h)2 (2 ?? 1) + 1)2 (3)
Specular G
We evaluated more options for the specular geometric attenuation term than any other. In the end,
we chose to use the Schlick model [19], but with k = /2, so as to better fit the Smith model for
GGX [21]. With this modification, the Schlick model exactly matches Smith for  = 1 and is a fairly
close approximation over the range [0, 1] (shown in Figure 2). We also chose to use Disney¡¯s modification
to reduce ¡°hotness¡± by remapping roughness using Roughness+1
2 before squaring. It¡¯s important to note
that this adjustment is only used for analytic light sources; if applied to image-based lighting, the
results at glancing angles will be much too dark.
k =
(Roughness + 1)2
8
G1(v) =
n  v
(n  v)(1 ?? k) + k
G(l; v; h) = G1(l)G1(v) (4)
Specular F
For Fresnel, we made the typical choice of using Schlick¡¯s approximation [19], but with a minor modification:
we use a Spherical Gaussian approximation [10] to replace the power. It is slightly more
efficient to calculate and the difference is imperceptible. The formula is:
F(v; h) = F0 + (1 ?? F0) 2 (??5:55473(vh)??6:98316)(vh) (5)
Where F0 is the specular reflectance at normal incidence.
3

================
Lazarov-Physically-Based-Lighting-in-Black-Ops (Siggraph 2011 Advances in Real-Time Rendering Course).pptx

ÏÂÔØµØÖ·
[25] Lazarov, ¡°Physically Based Lighting in Call of Duty: Black Ops¡± http://advances.realtimerendering.com/s2011/Lazarov-Physically-Based-Lighting-in-Black-Ops%20(Siggraph%202011%20Advances%20in%20Real-Time%20Rendering%20Course).pptx

²Î¿¼
Adopting a physically based shading model
https://seblagarde.wordpress.com/2011/08/17/hello-world/

ÄÚÈÝ
Primary Diffuse
Classic Lambert term 
Modulated by the shadow and the diffuse albedo
Secondary Diffuse
Reconstructed from lightmap/lightgrid secondary irradiance with per-pixel normal, modulated by the diffuse albedo

Primary Specular
Microfacet BRDF
Modulated by the shadow and the ¡°diffuse¡± cosine factor
Secondary Specular
Reconstructed from environment probe with per-pixel normal and Fresnel term, also tied to secondary irradiance
Based on same BRDF parameters as primary specular


Two textures: color and metalness
If metalness is 1 then color is treated as specular color and diffuse color is assumed to be black
If metalness is 0 then color is treated as diffuse color and specular color is assumed to be 0.03 linear

================
Adopting a physically based shading model
https://seblagarde.wordpress.com/2011/08/17/hello-world/

²Î¿¼
How to properly combine the diffuse and specular terms?
https://computergraphics.stackexchange.com/questions/2285/how-to-properly-combine-the-diffuse-and-specular-terms

In his largely referenced article on PBR, S¨¦bastien Lagarde even states that using (1?F) to weight the diffuse term is incorrect.


=============
Adopting a physically based shading model
https://seblagarde.wordpress.com/2011/08/17/hello-world/

Edit : This section is not up to date. Read Spherical Gaussian approximation for Blinn-Phong, Phong and Fresnel for full details.


Spherical Gaussian approximation for Blinn-Phong, Phong and Fresnel
https://seblagarde.wordpress.com/2012/06/03/spherical-gaussien-approximation-for-blinn-phong-phong-and-fresnel/

===============
Spherical Gaussian approximation for Blinn-Phong, Phong and Fresnel
https://seblagarde.wordpress.com/2012/06/03/spherical-gaussien-approximation-for-blinn-phong-phong-and-fresnel/

===============
Siggraph 2014 : Moving Frostbite to Physically based rendering V3
https://seblagarde.wordpress.com/tag/physically-based-rendering/

==============
Article - Physically Based Rendering
http://www.codinglabs.net/article_physically_based_rendering.aspx

Physics terms

If we want to properly understand the rendering equation we need to capture the meaning of some physical quantities; the most important of these quantities is called radiance (represented with L

in the formula). 
Radiance is a tricky thing to understand, as it is a combination of other physics quantities, therefore, before formally define it, we will introduce a few other quantities.

Radiant Flux: The radiant flux is the measure of the total amount of energy, emitted by a light source, expressed in Watts. We will represent the flux with the Greek letter ¦µ

. 
Any light source emits energy, and the amount of emitted energy is function of the wavelength. 
Figure 1: Daylight spectral distribution

In figure 1 we can see the spectral distribution for day light; the radiant flux is the area of the function (to be exact, the area is the luminous flux, as the graph is limiting the wavelength to the human visible spectrum). For our purposes we will simplify the radiant flux with an RGB colour, even if this means losing a lot of information. 

Solid angle: It's a way to measure how large an object appears to an observer looking from a point. To do this we project the silhouette of the object onto the surface of a unit sphere centred in the point we are observing from. The area of the shape we have obtained is the solid angle. In Figure 2 you can see the solid angle ¦Ø

as a projection of the light blue polygon on the unit sphere.
Figure 2: Solid angle
 

Radiant Intensity: is the amount of flux per solid angle. If you have a light source that emits in all directions, how much of that light (flux) is actually going towards a specific direction? Intensity is the way to answer to that, it's the amount of flux that is going in one direction passing through a defined solid angle. The formula that describes it is I=d¦µd¦Ø
, where ¦µ is the radiant flux and ¦Ø

is the solid angle.
Figure 3: Light intensity

Radiance: finally, we get to radiance. Radiance formula is:

L=d?2dAd¦Øcos¦È

=================
https://seblagarde.files.wordpress.com/2015/07/s2014_pbs_frostbite_slides.pdf

Siggraph 2014 : Moving Frostbite to Physically based rendering V3
https://seblagarde.wordpress.com/tag/physically-based-rendering/

==================
Rendering equation
https://en.wikipedia.org/wiki/Rendering_equation

Article - Physically Based Rendering
http://www.codinglabs.net/article_physically_based_rendering.aspx

================
Article - Physically Based Rendering - Cook¨CTorrance
http://www.codinglabs.net/article_physically_based_rendering_cook_torrance.aspx

 We are finally there, we can now put together the whole thing into an actual usable formula:

ks¡Ò¦¸DFG4(¦Øo?n)(¦Øi?n))Li(p,¦Øi)(n?¦Øi)d¦Øi¡Öks1N¡Æi=1NLi(¦Øi,p)F(¦Çi,¦Çt,h,¦Øo)G(¦Øi,¦Øo,h,n)sin(¦Èi)4|¦Øo?n||h?n|

That in code we translate to something like this:
float3 GGX_Specular( TextureCube SpecularEnvmap, float3 normal, float3 viewVector, float roughness, float3 F0, out float3 kS )
{
    float3 reflectionVector = reflect(-viewVector, normal);
    float3x3 worldFrame = GenerateFrame(reflectionVector);
    float3 radiance = 0;
    float  NoV = saturate(dot(normal, viewVector));

    for(int i = 0; i < SamplesCount; ++i)
    {
        // Generate a sample vector in some local space
        float3 sampleVector = GenerateGGXsampleVector(i, SamplesCount, roughness);
        // Convert the vector in world space
        sampleVector = normalize( mul( sampleVector, worldFrame ) );

        // Calculate the half vector
        float3 halfVector = normalize(sampleVector + viewVector);
        float cosT = saturatedDot( sampleVector, normal );
        float sinT = sqrt( 1 - cosT * cosT);

        // Calculate fresnel
        float3 fresnel = Fresnel_Schlick( saturate(dot( halfVector, viewVector )), F0 );
        // Geometry term
        float geometry = GGX_PartialGeometryTerm(viewVector, normal, halfVector, roughness) * GGX_PartialGeometryTerm(sampleVector, normal, halfVector, roughness);
        // Calculate the Cook-Torrance denominator
        float denominator = saturate( 4 * (NoV * saturate(dot(halfVector, normal)) + 0.05) );
        kS += fresnel;
        // Accumulate the radiance
        radiance += SpecularEnvmap.SampleLevel( trilinearSampler, sampleVector, ( roughness * mipsCount ) ).rgb * geometry * fresnel * sinT / denominator;
    }

    // Scale back for the samples count
    kS = saturate( kS / SamplesCount );
    return radiance / SamplesCount;        
}

By using this Monte Carlo estimator we can evaluate how much light is reflected by the surface and we can then add it to the diffuse component that we have calculated using Lambert. The last thing we need now is to calculate the two weights kd
and ks. Since these weights represent the amount of light reflected it's natural to immediately think of fresnel. In fact we can use fresnel itself for ks and then, for the energy conservation law, we can derive kd as kd=1?ks

. It's important to notice that in the GGX calculation we have already multiplied the radiance by fresnel, so in the final formula we won't be doing it again.
float4 PixelShaderFunction(VertexShaderOutput input) : SV_TARGET0
{
    ...

    float3 surface = tex2D(surfaceMap_Sampler, input.Texcoord).rgb;   
    float ior = 1 + surface.r;
    float roughness = saturate(surface.g - EPSILON) + EPSILON;
    float metallic = surface.b;

    // Calculate colour at normal incidence
    float3 F0 = abs ((1.0 - ior) / (1.0 + ior));
    F0 = F0 * F0;
    F0 = lerp(F0, materialColour.rgb, metallic);
        
    // Calculate the specular contribution
    float3 ks = 0;
    float3 specular = GGX_Specular(specularCubemap, normal, viewVector, roughness, F0, ks );
    float3 kd = (1 - ks) * (1 - metallic);
    // Calculate the diffuse contribution
    float3 irradiance = texCUBE(diffuseCubemap_Sampler, normal ).rgb;
    float3 diffuse = materialColour * irradiance;

    return float4( kd * diffuse + /*ks **/ specular, 1);     
}

Also, note that kd

is weighted by (1-metallic). This is to simulate the fact that a metallic surface doesn't diffuse light at all, so it can't have a diffuse component.

The final results can be seen in the images below. This is the model lit in different lighting conditions:

 References

[1] Walter et al. "Microfacet Models for Refraction through Rough Surfaces"
[2] Lazanyi, Szirmay-Kalos, ¡°Fresnel term approximations for Metals¡±

==================
Microfacet Models for Refraction through Rough Surfaces
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.html
http://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.pdf

===================
Fresnel term approximations for Metals
https://www.researchgate.net/publication/221546550_Fresnel_Term_Approximations_for_Metals

https://www.researchgate.net/profile/Laszlo_Szirmay-Kalos/publication/221546550_Fresnel_Term_Approximations_for_Metals/links/09e41510830d877b0f000000/Fresnel-Term-Approximations-for-Metals.pdf

==============
EGSR07-btdf.pdf

3.1. Microfacet Distribution Function, D
The microfacet normal distribution, D(m), describes the statistical
distri


3.2. Shadowing-Masking Function, G
The bidirectional shadowing-masking function G(i,o,m)

A wide variety of microfacet distribution functions D
have been proposed. In this paper, we discuss three different
types: Beckmann, Phong, and GGX.

================
Siggraph 2014 : Moving Frostbite to Physically based rendering V3
https://seblagarde.wordpress.com/2015/07/14/siggraph-2014-moving-frostbite-to-physically-based-rendering/

http://www.cs.virginia.edu/~jdl/bib/appearance/analytic%20models/he91.pdf
http://www.cs.cornell.edu/~srm/publications/egsr07-btdf.pdf
http://www.geometrictools.com/Documentation/DistanceToCircle3.pdf
http://holger.dammertz.org/stuff/notes_HammersleyOnHemisphere.html

getSample is a GPU random number generator,
It is implemented to generate a stochastic samples to reduce the number of samples required to get good result.

A typical implementation will use Hammersley on GPU

http://holger.dammertz.org/stuff/notes_HammersleyOnHemisphere.html

float radicalInverse_VdC(uint bits) {
bits = (bits <> 16u);
bits = ((bits & 0x55555555u) <> 1u);
bits = ((bits & 0x33333333u) <> 2u);
bits = ((bits & 0x0F0F0F0Fu) <> 4u);
bits = ((bits & 0x00FF00FFu) <> 8u);
return float(bits) * 2.3283064365386963e-10; // / 0x100000000
}

vec2 hammersley2d(uint i, uint N) {
return vec2(float(i)/float(N), radicalInverse_VdC(i));
}

=================
s2014_pbs_frostbite_slides.pdf

Our#specular#term#is#a#tradi1onal#microfacet#model,#using#Schlick¡¯s#approxima1on#of#
the#Fresnel#func1on,#and#the#GGX#Normal#Distribu1on#Func1on#(NDF).#

Here#is#a#simple#comparison.#First#the#uncorrelated#Smith#G#term,#for#a#dielectric#
material#with#black#diffuse#(top)#and#a#metal#material#(boSom).#

We#have#inves1gated#proper#deriva1ons#from#the#GGX#distribu1on#as#[Gotanda14],#
but#we#went#for#Disney¡¯s#diffuse#model#(from#[Burley12])#as#it#is#simple#and#good#
enough.#

As#a#quick#reminder#of#Disney¡¯s#diffuse#model,#here#is#a#comparison.#This#is#
Lamber1an#diffuse,#which#is#the#same#for#all#roughness#values.#

This#covers#a#few#types:#
O#A#distant#light#probe#for#parallaxOfree#far#ligh1ng#
O#Local#light#probes,#for#local#ligh1ng,#with#parallax#
O#Screen#space#reflec1ons,#for#closeOrange#ligh1ng#(suppor1ng#glossy#reflec1on)#
O#Planar#reflec1ons#as#an#alterna1ve#to#SSR#

References
Brent Burley, "Physically Based Shading at Disney" SIGGRAPH12, PBR Course
Brain Karis, "Real Shading in Unreal Engine 4" , SIGRRAPH3, PBR Course

==============
bing 	Real Shading in Unreal Engine 4
Real Shading in Unreal Engine 4
https://cdn2.unrealengine.com/Resources/files/2013SiggraphPresentationsNotes-26915738.pdf

===============
bing	Physically Based Shading at Disney
Physically Based Shading at Disney
http://blog.selfshadow.com/publications/s2012-shading-course/burley/s2012_pbs_disney_brdf_notes_v3.pdf

===============
s2012_pbs_disney_brdf_notes_v3.pdf

To examine the MERL measured materials and compare with analytic models, we developed a new
tool, the BRDF Explorer, shown in Figure 2. It is available as open source at github.com/wdas/brdf
and has the following features:

github.com/wdas/brdf

ºÜ¶àºÃµÄ×ÊÔ´


Commit

Correct (anisotropic) GGX Smith G function
selfshadow committed on 23 Feb 2017

This modification yields more correct behaviour for anisotropic materials and removes the previous ad hoc roughness remapping (roughness*.5 + .5). This better reflects current practice at Disney, as discussed in the ¡°Specular G revisited¡± addendum of the ¡°Physically Based Shading at Disney¡± SIGGRAPH¡¯12 course notes (http://blog.selfshadow.com/publications/s2012-shading-course/).


http://blog.selfshadow.com/publications/s2012-shading-course/

==========================
http://blog.selfshadow.com/publications/s2012-shading-course/

09:00 Introduction: The Importance of Physically Based Shading (Stephen Hill) [slides: ppt, pdf]
09:05 Background: Physics and Math of Shading (Naty Hoffman) [slides] [course notes] [notebook: mathematica, pdf]
09:30 Calibrating Lighting and Materials in Far Cry 3 (Stephen McAuley) [slides: ppt, pdf] [video] [course notes]
10:00 Beyond a Simple Physically Based Blinn-Phong Model in Real-Time (Yoshiharu Gotanda) [slides: ppt, pdf] [course notes]
10:30 Break
10:45 Physical Production Shaders with OSL (Adam Martinez) [slides] [course notes]
11:15 Physically Based Shading at Disney (Brent Burley) [slides: keynote, pdf] [course notes]
11:45 Reflection Model Design for WALL-E and Up (Brian Smits) [slides: keynote, pdf] [notebook: mathematica, pdf] 

===============
On Filtering the Noise from the Random Parameters
in Monte Carlo Rendering
http://cvc.ucsb.edu/graphics/Papers/Sen2011_RPF/

================
Publications
http://blog.selfshadow.com/publications/

Physically Based Shading in Theory and Practice (SIGGRAPH 2017)
Physically Based Shading in Theory and Practice (SIGGRAPH 2016)
Physically Based Shading in Theory and Practice (SIGGRAPH 2015)
Physically Based Shading in Theory and Practice (SIGGRAPH 2014)
Physically Based Shading in Theory and Practice (SIGGRAPH 2013)
Practical Physically Based Shading in Film and Game Production (SIGGRAPH 2012)

================
SIGGRAPH 2016 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2016-shading-course/

14:00 Recent Advances in Physically Based Shading (Naty Hoffman) [slides: pdf]
14:20 Unified Shading and Asset Development at Lucasfilm and ILM (Roger Cordes and Dan Lobl)
15:00 Physically Based Sky, Atmosphere and Cloud Rendering in Frostbite (S¨¦bastien Hillaire) [slides: ppt]
15:30 Break
15:45 An Artist-Friendly Workflow for Panoramic HDRI (S¨¦bastien Lagarde) [slides: ppt, pdf] [course notes] [supplemental]
16:05 Physically Based Hair Shading in Unreal (Brian Karis) [slides: ppt, pdf]
16:25 Practical Real-Time Strategies for Accurate Indirect Occlusion (Jorge Jim¨¦nez) [slides: ppt, pdf]
16:45 Towards Bidirectional Path Tracing at Pixar (Christophe Hery and Ryusuke Villemin) [course notes]

===============
SIGGRAPH 2017 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2017-shading-course/

14:00 Real-Time Line- and Disk-Light Shading (Eric Heitz and Stephen Hill) [slides]
14:30 Physically Based Shading at DreamWorks Animation (Feng Xie and Jon Lanz) [course notes]
15:00 Volumetric Skin and Fabric Shading at Framestore (Nathan Walster) [slides] [course notes]
15:30 Break
15:45 Practical Multilayered Materials in Call of Duty: Infinite Warfare (Micha? Drobot) [slides: ppt, pdf]
16:05 Pixar¡¯s Foundation for Materials: PxrSurface and PxrMarschnerHair (Christophe Hery and Junyi Ling) [course notes]
16:35 Revisiting Physically Based Shading at Imageworks (Christopher Kulla and Alejandro Conty) [slides] [supplemental] 

=================
SIGGRAPH 2013 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2013-shading-course/

09:00 Introduction (Stephen Hill)
09:05 Background: Physics and Math of Shading (Naty Hoffman) [slides] [course notes] [notebook: mathematica, pdf]
09:20 Getting More Physical in Call of Duty: Black Ops II (Dimitar Lazarov) [slides: ppt, pdf] [course notes] [notebook]
09:40 Real Shading in Unreal Engine 4 (Brian Karis) [slides: ppt, pdf] [course notes]
10:00 Crafting a Next-Gen Material Pipeline for The Order: 1886 (David Neubelt & Matt Pettineo) [slides: ppt, pdf] [course notes] [video] [code]
10:30 Break
10:45 Everything You Always Wanted to Know About mia_material (Zap Andersson) [slides: ppt, pdf] [course notes]
11:10 OSL The Great and Powerful (Adam Martinez) [slides]
11:35 Physically Based Shading at Pixar (Christophe Hery & Ryusuke Villemin) [slides] [course notes] 

==============
SIGGRAPH 2014 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2014-shading-course/

14:00 Physics and Math of Shading (Naty Hoffman) [slides]
14:20 Understanding the Masking-Shadowing Function (Eric Heitz) [slides] [course notes]
14:40 Antialiasing Physically Based Shading with LEADR Mapping (Jonathan Dupuy) [slides]
15:00 Designing Reflectance Models for New Consoles (Yoshiharu Gotanda)
15:30 Break
15:45 Moving Frostbite to PBR (S¨¦bastien Lagarde & Charles de Rousiers) [slides: pptx, pdf]
16:15 Physically Based Shader Design in Arnold (Anders Langlands) [slides] [course notes]
16:35 Art Direction within Pixar¡¯s Physically Based Lighting System (Ian Megibben & Farhez Rayani) 

================
SIGGRAPH 2015 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2015-shading-course/

09:00 Introduction
09:05 Physics and Math of Shading (Naty Hoffman) [slides]
09:20 layerlab: A Computational Toolbox for Layered Materials (Wenzel Jakob) [slides] [course notes]
09:40 Approximate Models for Physically Based Rendering (Micha? Iwanicki & Angelo Pesce) [slides]
10:00 Real-World Measurements for Call of Duty: Advanced Warfare (Danny Chan) [course notes]
10:30 Break
10:45 Advanced Lighting R&D at Ready At Dawn Studios (David Neubelt & Matt Pettineo) [slides: ppt, pdf]
11:15 Extending the Disney BRDF to a BSDF with Integrated Subsurface Scattering (Brent Burley) [slides: keynote, pdf] [course notes]
11:45 Physically Based Material Modeling at Weta Digital (Luca Fascione) 

===================
bing	GGX_height_correlated

================
PBR Diffuse Lighting for 
GGX+Smith
Microsurfaces
http://twvideo01.ubm-us.net/o1/vault/gdc2017/Presentations/Hammon_Earl_PBR_Diffuse_Lighting.pdf

===============
Ogre vs Unity BRDF #545
https://github.com/OGRECave/ogre/issues/545

===============
Unreal Insight£ºÕæÊµ½ÇÉ«äÖÈ¾
http://gad.qq.com/article/detail/28536

ÈçÉÏÍ¼£¬DÏî½«Beckmann·Ö²¼ÖÐµÄtanÏîµ¹ÖÃµÃµ½cotÏî£¬µÃµ½InverseGauss·Ö²¼º¯Êý£¬¸Ã·Ö²¼º¯ÊýÂú×ãÁË²¼ÁÏ¹Û²ìµÃµ½µÄÄÜÁ¿·Ö²¼ÐÎÊ½¡£

ÔÚUE4µÄShader´úÂëÖÐ£¬ClothShadingÕýÊÇÊÜ¸Ã·½·¨Æô·¢£¬¸ÄÔìGGXµÃµ½InvGGXº¯Êý×÷Îª²¼ÁÏäÖÈ¾ÖÐµÄDÏî¡£

ÎÒÃÇÀ´¿´ÏÂUE4ShadersÄ¿Â¼ÏÂShadingModels.usfµÄClothShading´úÂë£º
// Cloth - Asperity Scattering - Inverse Beckmann Layer 
    float3 F1 = F_Schlick( FuzzColor, VoH );
    float  D1 = D_InvGGX( LobeRoughness[1], NoH ); // UE4 ClothShadingÄ£ÐÍÖÐÔö¼ÓÁË²¼ÁÏ´Ö²Ú±íÃæÉ¢ÉäµÄÏî
                                                   // Õâ¸ö·½·¨ÊÇÍ¨¹ý¹Û²ì²¼ÁÏµÃµ½µÄ
    float  V1 = Vis_Cloth( NoV, NoL );
    float3 Spec1 = D1 * V1 * F1;
    // Generalized microfacet specular
    float3 F2 = F_Schlick( GBuffer.SpecularColor, VoH );
    float  D2 = D_GGX( LobeRoughness[1], NoH ) * LobeEnergy[1];
    float  V2 = Vis_SmithJointApprox( LobeRoughness[1], NoV, NoL );
    float3 Spec2 = D2 * V2 * F2;
    float3 Spec = lerp(Spec2, Spec1, Cloth);
    return Diff + Spec;
	
Æ¤·ôäÖÈ¾

ÔÚUE4ÖÐ£¬´Î±íÃæÉ¢ÉäµÄ¼ÆËãÊµÏÖºÍÉÏÃæÌáµ½µÄJorgeJimenezÌá³öµÄ·½·¨ÀàËÆ£¬Í¨¹ýÔÚÆÁÄ»¿Õ¼ä ¾í»ý´Î±íÃæµÄÉî¶ÈÌùÍ¼£¬ÒÀ¾Ý¹âÔ´µÄÎ»ÖÃºÍÉ¢Éä°ë¾¶¼ÆËã³öÉ¢ÉäÑÕÉ«¡£

ÒÔÏÂÊÇJorgeJimenez¸ø³öµÄÑùÀý´úÂë£¬ÏêÏ¸ÊµÏÖ¿É²Î¿¼Github

²Î¿¼×ÊÁÏ
Real Shading in Unreal Engine 4
PBR Theory
Arbitrarily Layered Micro-Facet Surfaces
Moving Frostbite to Physically Based Rendering
Importance Sampling for Physically-Based Hair Fiber Models
Light Scattering from Human Hair Fibers
Photorealistic Character
Physically Based Hair Shading in Unreal
Screen-Space Perceptual Rendering of Human Skin
Distribution-based BRDFs
Crafting a Next-Gen Material Pipeline for The Order: 1886
Unreal Engine 4¸øParagon½ÇÉ«¸³ÓèÉúÃü



https://learnopengl.com/PBR/Theory
https://www.cg.tuwien.ac.at/research/publications/2007/weidlich_2007_almfs/weidlich_2007_almfs-paper.pdf
https://cg.ivd.kit.edu/publications/pubhanika/2013_hairbrief.pdf
http://www.graphics.stanford.edu/papers/hair/hair-sg03final.pdf
https://docs.unrealengine.com/en-us/Resources/Showcases/PhotorealisticCharacter?utm_source=launcher&utm_medium=ue&utm_campaign=uelearn
http://www.iryoku.com/sssss/
http://www.cs.utah.edu/%7Epremoze/dbrdf/dBRDF.pdf
http://blog.selfshadow.com/publications/s2013-shading-course/rad/s2013_pbs_rad_slides.pdf
http://mp.weixin.qq.com/s/lF34ypY8pVnp_9W-WvC5kg


==================
Separable Subsurface Scattering is a technique that allows to efficiently perform subsurface scattering calculations in screen space in just two passes. http://www.iryoku.com/
https://github.com/iryoku/separable-sss

²Î¿¼
Unreal Insight£ºÕæÊµ½ÇÉ«äÖÈ¾
http://gad.qq.com/article/detail/28536

Æ¤·ôäÖÈ¾

ÔÚUE4ÖÐ£¬´Î±íÃæÉ¢ÉäµÄ¼ÆËãÊµÏÖºÍÉÏÃæÌáµ½µÄJorgeJimenezÌá³öµÄ·½·¨ÀàËÆ£¬Í¨¹ýÔÚÆÁÄ»¿Õ¼ä ¾í»ý´Î±íÃæµÄÉî¶ÈÌùÍ¼£¬ÒÀ¾Ý¹âÔ´µÄÎ»ÖÃºÍÉ¢Éä°ë¾¶¼ÆËã³öÉ¢ÉäÑÕÉ«¡£

ÒÔÏÂÊÇJorgeJimenez¸ø³öµÄÑùÀý´úÂë£¬ÏêÏ¸ÊµÏÖ¿É²Î¿¼Github

=================
Marschner
http://www.graphics.stanford.edu/papers/hair/hair-sg03final.pdf

²Î¿¼
Unreal Insight£ºÕæÊµ½ÇÉ«äÖÈ¾
http://gad.qq.com/article/detail/28536

Í··¢¹âÕÕ

ParagonÖÐµÄÍ··¢¹âÏß´«²¥Ä£ÐÍÊÇ»ùÓÚMarschnerµÄµ¥ÌõÍ··¢Â·¾¶½¨Ä£µÄ¡£

==============
https://docs.unrealengine.com/en-us/Engine/Rendering/Materials/PhysicallyBased
References

1. Lagarde, Feeding a physically based shading model
http://seblagarde.wordpress.com/2011/08/17/feeding-a-physical-based-lighting-mode/
2. Karis, Real Shading in Unreal Engine 4
https://de45xmedrsdbp.cloudfront.net/Resources/files/2013SiggraphPresentationsNotes-26915738.pdf
3. Burley, Physically-Based Shading at Disney
http://blog.selfshadow.com/publications/s2012-shading-course/burley/s2012_pbs_disney_brdf_slides_v2.pdf
4. Smits, Reflection Model Design for WALL-E and Up
http://blog.selfshadow.com/publications/s2012-shading-course/smits/s2012_pbs_pixar_model_slides_v2.pdf
5. Hable, Everything is Shiny
http://www.filmicgames.com/archives/547

==============
SIGGRAPH 2013 Course: Physically Based Shading in Theory and Practice
http://blog.selfshadow.com/publications/s2013-shading-course/#course_content

Syllabus

09:00 Introduction (Stephen Hill)
09:05 Background: Physics and Math of Shading (Naty Hoffman) [slides] [course notes] [notebook: mathematica, pdf]
09:20 Getting More Physical in Call of Duty: Black Ops II (Dimitar Lazarov) [slides: ppt, pdf] [course notes] [notebook]
09:40 Real Shading in Unreal Engine 4 (Brian Karis) [slides: ppt, pdf] [course notes]
10:00 Crafting a Next-Gen Material Pipeline for The Order: 1886 (David Neubelt & Matt Pettineo) [slides: ppt, pdf] [course notes] [video] [code]
10:30 Break
10:45 Everything You Always Wanted to Know About mia_material (Zap Andersson) [slides: ppt, pdf] [course notes]
11:10 OSL The Great and Powerful (Adam Martinez) [slides]
11:35 Physically Based Shading at Pixar (Christophe Hery & Ryusuke Villemin) [slides] [course notes] 

ref
UE4ÊÇÈçºÎ¼ÆËãµã¹âÔ´£¬Æ½ÐÐ¹âÔ´²úÉúµÄ×îÖÕÑÕÉ«µÄ£¿
http://www.opengpu.org/forum.php?mod=viewthread&tid=18720
http://blog.selfshadow.com/publi ... s_epic_notes_v2.pdf

==============
PBR Theory
https://learnopengl.com/PBR/Theory

Further reading
Background: Physics and Math of Shading by Naty Hoffmann: there is too much theory to fully discuss in a single article so the theory here barely scratches the surface; if you want to know more about the physics of light and how it relates to the theory of PBR this is the resource you want to read.
Real shading in Unreal Engine 4: discusses the PBR model adopted by Epic Games in their 4th Unreal Engine installment. The PBR system we'll focus on in these tutorials is based on this model of PBR.
Marmoset: PBR Theory: an introduction to PBR mostly meant for artists, but nevertheless a good read.
Coding Labs: Physically based rendering: an introduction to the render equation and how it relates to PBR.
Coding Labs: Physically Based Rendering - Cook¨CTorrance: an introduction to the Cook-Torrance BRDF.
Wolfire Games - Physically based rendering: an introduction to PBR by Lukas Orsv?rn.
[SH17C] Physically Based Shading: a great interactive shadertoy example (warning: might take a while to load) by Krzysztof Narkowi showcasing light-material interaction in a PBR fashion.


https://www.marmoset.co/toolbag/learn/pbr-theory
http://www.codinglabs.net/article_physically_based_rendering.aspx
http://www.codinglabs.net/article_physically_based_rendering_cook_torrance.aspx
http://blog.wolfire.com/2015/10/Physically-based-rendering
https://www.shadertoy.com/view/4sSfzK


==============
Photorealistic Character
https://docs.unrealengine.com/en-us/Resources/Showcases/PhotorealisticCharacter?utm_source=launcher&utm_medium=ue&utm_campaign=uelearn

=============
Screen-Space Perceptual Rendering of Human Skin
http://www.iryoku.com/sssss/

Screen-space skin rendering is being used in Unreal Engine 3 and Unigine! More in The Technology Behind the DirectX 11 Unreal Engine and in the Unigine Dev Blog.

Related

2010: Real-Time Realistic Skin Translucency
2010: A Practical Appearance Model for Dynamic Facial Color
2011: Practical and Realistic Facial Wrinkles Animation
2015: Separable Subsurface Scattering

Links

March 10, 2010: Piel virtual que acaricia al espectador (Heraldo de Arag¨®n), in Spanish
March 10, 2010: Hollywood se fija en la Universidad de Zaragoza (Heraldo de Arag¨®n), in Spanish


Screen-space skin rendering is being used in Unreal Engine 3 and Unigine! More in The Technology Behind the DirectX 11 Unreal Engine and in the Unigine Dev Blog.
http://www.nvidia.com/content/PDF/GDC2011/GDC2011EpicNVIDIAComposite.pdf
https://developer.unigine.com/devlog/
















