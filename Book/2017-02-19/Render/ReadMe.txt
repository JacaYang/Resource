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

=====================
Unity5 GIÓëPBSäÖÈ¾´ÓÓÃ·¨µ½×ÅÉ«´úÂë
https://www.cnblogs.com/zhouxin/p/5168632.html
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

























