# Reading list




**To add**


* On software packages
    * Eklund et al - Does parametric fMRI analysis with SPM yield valid results? — An empirical study of 1484 rest datasets
    * Groenensschild et al - The Effects of FreeSurfer Version, Workstation Type, and Macintosh Operating System Version on Anatomical Volume and Cortical Thickness Measurements
* On the limits of fMRI:
    * Logotetis - what you can and what you cannot do with fMRI
    * Cacioppo
* Voodoo correlation
* The seductive allure of brain scans
* On knowing where your activation is
    * Devlin, Joseph T & Russell Poldrack, 2007, Neuroimage, In praise of tedious anatomy



link to ressource sections

papers on Reproducibility
papers on inferences
power, number of participants necessary, reliability (resampling from connectome project)

link to Tal's response to Friston
link to tal's paper on why small studies give big correlations
link to law of small numbers paper by kanheman
link to figures of scanning the horizon


papers for beginners

LAuren atlas paper on pain
Cyril on GLM
Cacioppo
What you can and cannot do with fMRI by lokothetis

robustness checks


Chamberlin multiple hypothesis
Forscher chaos in the brickyard
Platt's strong inference
Hedge on hard/soft science
and the come back on if psych is soft it is for a good reason


*Here, we outline the basic areas of knowledge that we think are essential to becoming an expert at fMRI analysis, roughly in order of importance.*

1. *Probability and statistics. There is probably no more important foundation for fMRI analysis than a solid background in basic probability and statistics. Without this, nearly all of the concepts that are central to fMRI analysis will be foreign.*
2. *Computer programming. It is our opinion that one simply cannot become an effective user of fMRI analysis without strong computer programming skills. There are many languages that are useful for fMRI analysis, including MATLAB, Python, and UNIX shell scripting. The particular language is less important than an underlying understanding of the methods of programming, and this is a place where practice really does make perfect, particularly with regard to debugging programs when things go wrong.*
3. *Linear algebra. The importance of linear algebra extends across many different aspects of fMRI analysis, from statistics (where the general inear model is most profitably defined in terms of linear algebra) to image processing (where many operations on images are performed using linear algebra). A deep understanding of fMRI analysis requires basic knowledge of linear algebra.*
4. *Magnetic resonance imaging. One can certainly analyze fMRI data without knowing the details of MRI acquisition, but a full understanding of fMRI data requires that one understand where the data come from and what they are actually measuring. This is particularly true when it comes to understanding the various ways in which MRI artifacts may affect data analysis.*
5. *Neurophysiology and biophysics. fMRI signals are interesting because they are an indirect measure of the activity of individual neurons. Understanding how neurons code information, and how these signals are reflected in blood flow, is
crucial to interpreting the results that are obtained from fMRI analysis.*
6. *Signal and image processing. A basic understanding of signal and image processing methods is important for many of the techniques discussed in this book. In particular, an understanding of Fourier analysis is very useful for nearly every aspect of fMRI analysis.*


http://jonathanpeelle.net/mri-reading-list
https://www.scienceopen.com/search#collection/873f3e77-23c2-4586-bf82-9985a55a0894
https://www.fil.ion.ucl.ac.uk/spm/doc/spmbib.html

**Table of Contents**

* [Refresh your maths](#Refresh-your-maths)
* [Refresh your physics](#)
* [Reproducibility](#Reproducibility)
* [Data sharing](#)
* [analytic flexibility](#)
* [Experimental design](#)
* [Power](#Power)
* [Design efficiency](#)
* [Realignement](#Realignement)
* [Unwarping](#Unwarping)
* [Slice timing](#)
* [Scrubbing](#Scrubbing)
* [Smoothing](#Smoothing)
* [Preprocessing](#Preprocessing)
* [Quality control](#)
* [GLM](#GLM)
* [Correction for multiple comparisons](#)
* [Effect size and percent signal change](#)
* [Circularity](#Circularity)
* [Anatomical localization](#)
* [Multivariate analysis](#)
* [High-resolution MRI](#)
* [Reporting](#Reporting)
* [Meta analysis](#)


Big picture papers
list of historical papers
can a neuroscientist understand a microprocessor?
Cacioppo's





which atlas to choose
son: http://sci-hub.tw/http://www.sciencedirect.com/science/article/pii/S1053811917303026 31



Statistics and inferences
strong inference
meehl
cohen


## Reproducibility

Here is a blog post on how running the same analysis on different versions of FSL or different of Mac OS gives... different results:
- http://neuroskeptic.blogspot.co.uk/2012/06/brains-are-different-on-macs.html .

reproducibility manifesto

Pernet CR, Poline J-B (2015) Improving functional magnetic resonance imaging reproducibility. GigaScience 4:15. http://dx.doi.org/10.1186/s13742-015-0055-8

Poldrack RA, Baker CI, et al. (2017) Scanning the horizon: towards transparent and reproducible neuroimaging research. Nature Reviews Neuroscience 18:115-126. https://doi.org/10.1038/nrn.2016.167

## Data sharing

bids
neurovault
NIDM

Gorgolewski KJ, Varoquaux G, Rivera G, Schwarz Y, Ghosh SS, Maumet C, Sochat VV, Nichols TE, Poldrack RA, Poline J-B, Yarkoni T, Margulies DS (2015) NeuroVault.org: a web-based repository for collecting and sharing unthresholded statistical maps of the human brain. Front Neuroinform 9:8. http://dx.doi.org/10.3389/fninf.2015.00008

Poldrack RA, Gorgolewski KJ (2017) OpenfMRI: Open sharing of task fMRI data. NeuroImage 144:259-261. https://doi.org/10.1016/j.neuroimage.2015.05.073


## Analytic flexibility

Given how many parameters can be changed in the pre-processing pipelines, the number of the researcher's degree of freedom can allow to show quite different results on the same data:
- http://blogs.discovermagazine.com/neuroskeptic/2012/10/14/more-on-false-positive-neuroimaging .


Carp J (2012) On the plurality of (methodological) worlds: Estimating the analytic flexibility of fMRI experiments. Frontiers in Neuroscience 6:1-13. https://doi.org/10.3389/fnins.2012.00149

Simmons JP, Nelson LD, Simonsohn U (2011) False-positive psychology: Undisclosed flexibility in data collection and analysis allows presenting anything as significant. Psychological Science 22:1359-1366. https://doi.org/10.1177/0956797611417632


## Experimental design

You will find more information in this chapter of the SPM manual: Chapter_Experimental_Design.pdf

The "pure insertion assumption" (the assumption that there is no interaction between experimental factors), mentioned in this lecture, is conceptually related to a statistical analysis error that was recently shown to be quite widespread in neuroscience (http://www.nature.com/neuro/journal/v14/n9/full/nn.2886.html). For a lighter read, here are two blog posts about it:

- http://www.theguardian.com/commentisfree/2011/sep/09/bad-science-research-error.
- http://bigthink.com/Mind-Matters/study-a-lot-of-mind-and-brain-research-depends-on-flawed-statistics

same analysis approach carsten



## Power

gigerenzer
mindless rituals
no increase in power in 60 years

mumford
https://academic.oup.com/scan/article/7/6/738/1646637

power failure
Tal's paper in response to the voodoo thing

Liu TT, Frank LR (2004) Efficiency, power, and entropy in event-related FMRI with multiple trial types: Part I: theory. NeuroImage 21:387-400. http://doi.org/10.1016/j.neuroimage.2003.09.030

Liu TT (2004) Efficiency, power, and entropy in event-related fMRI with multiple trial types Part II: Design of experiments. NeuroImage 21:401–413. http://dx.doi.org/10.1016/j.neuroimage.2003.09.031

## Design efficiency
Dale


## Realignement

Mangin How SPM can create spurious activation

Power JD, Barnes KA, Snyder AZ, Schlaggar BL, Petersen SE (2012) Spurious but systematic correlations in functional connectivity MRI networks arise from subject motion. NeuroImage 59:2142-2154. http://dx.doi.org/10.1016/j.neuroimage.2011.10.018

Siegel JS, Power JD, Dubis JW, Vogel AC, Church JA, Schlaggar BL, Petersen SE (2014) Statistical improvements in functional magnetic resonance imaging analyses produced by censoring high-motion data points. Hum Brain Mapp 35:1981-1996. http://dx.doi.org/10.1002/hbm.22307

On the importance of head movement correction (the peer reviewed papers are referenced in the blog posts):
- in functionnal connectivty analysis: http://neuroskeptic.blogspot.co.uk/2011/07/brain-connectivity-or-head-movement.html .
- in tractography studies: http://blogs.discovermagazine.com/neuroskeptic/2013/11/26/head-movement-bad-news-neuroscience
On why there might be some residual effects of movement in your data even after realigning (AKA "spin history effect") and why you should always add your realignment parameters as regressors of no interest to correct for that effect: I suggest reading this article (http://cream.fil.ion.ucl.ac.uk/spm/doc/papers/fMRI_1/fMRI_1.pdf) where the following passage is from.

*Time-dependent changes in a fMRI signal, at a given point in the brain, have many components. This paper is concerned with movement-related components. These components can arise from:*
* *Differences in the position of the object in the scanner Spatial variation in sensitivity will render the signal a function of the object's position at the time of scanning. This spatial variability can include large scale field inhomogeneity or can be expressed at a much finer scale. An important example of the latter is found in slice-selective irradiation, used for example in multi-slice acquisition. The degree to which spins are excited in any small volume of the object will depend on an interaction between the local magnetic field and the Fourier transform of the slice-selective pulse. For example the excitation of spins in a small region on the edge of a slice will be exquisitely sensitive to small displacements in and out of that slice. In other words signal intensity will be a strong function of position relative to the volume excited or the scanner's frame of reference.*
* *Differences due to the history of the position of the object. If the number of excited spins is a function of position in the scanner it follows that the number of excited spins (and implicitly the signal) will also be a function of position in previous scans. This dependency is due to changes in saturation of spin magnetization, that is a function of the number of spins excited in the previous scan. This excitation will in turn be a function of position and so, by induction, a function of all previous positions. In summary the current signal is a function of current position and the spin excitation history. The spin excitation history is in turn determined by the history of past movements. This effect will manifest if the recovery of magnetization in the z direction is incomplete by the time the next slice-selective pulse arrives (i.e. if TR is comparable to T1 which is certainly the case for many fMRI studies). In general movement within the plane of the slice will not change the set of spins excited and should not contribute to this effect.*



## Unwarping

On unwarping : this passage of the SPM manual might help you understand what this problem this preprocessing tries to solve and how it does it.

*EPI images are not particularly faithful reproductions of the object, and in particular there are severe geometric distortions in regions where there is an air-tissue interface (e.g. orbitofrontal cortex and the anterior medial temporal lobes). In these areas in particular the observed image is a severely warped version of reality, much like a funny mirror at a fair ground. When one moves in front of such a mirror ones image will distort in different ways and ones head may change from very elongated to seriously flattened. If we were to take digital snapshots of the reflection at these different positions it is rather obvious that realignment will not suffice to bring them into a common space.
The situation is similar with EPI images, and an image collected for a given subject position will not be identical to that collected at another. We call this effect susceptibility-by-movement interaction. Unwarp is predicated on the assumption that the susceptibility-by- movement inter-action is responsible for a sizable part of residual movement related variance. Assume that we know how the deformations change when the subject changes position (i.e. we know the derivatives of the deformations with respect to subject position). That means that for a given time series and a given set of subject movements we should be able to predict the ”shape changes” in the object and the ensuing variance in the time series. It also means that, in principle, we should be able to formulate the inverse problem, i.e. given the observed variance (after realignment) and known (estimated) movements we should be able to estimate how deformations change with subject movement. We have made an attempt at formulating such an inverse model, and at solving for the ”derivative fields”. A deformation field can be thought of as little vectors at each position in space showing how that particular location has been deflected. A ”derivative field” is then the rate of change of those vectors with respect to subject movement. Given these ”derivative fields” we should be able to remove the variance caused by the susceptibility-by-movement interaction. Since the underlying model is so restricted we would also expect experimentally induced variance to be preserved.*



## Slice timing
This article (http://www.sciencedirect.com/science/article/pii/S1053811911007245). shows data suggesting it always better to slice-timing correct your data (especially if you have an event-related protocol and long TRs).

Sladky R, Friston KJ, Tröstl J, Cunnington R, Moser E, Windischberger C (2011) Slice-timing effects and their correction in functional MRI. NeuroImage 58:588-594. http://dx.doi.org/10.1016/j.neuroimage.2011.06.078

## Scrubbing



## Smoothing
If you are still unclear about how smoothing works and what the match filter theorem is, have a look at the page below. There is also another good visual example of how convolution works.
- http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesSmoothing

Turner: problems with current fMRI analysis


## Preprocessing
fMRIprep


## Quality control
power plot
MRIQC

## GLM
More information on the implementation of the GLM and the visualization of design matrices in SPM.

- http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesStatistics

This article (http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896880/)Links to an external site. has some good things to say on the the use of GLM in fMRI and explains in a bit more detail some issues. It also comes with a set of matlab scripts to run some simulations to drive the point home.

mumford on orthogonalization



Pernet CR (2014) Misconceptions in the use of the General Linear Model applied to functional MRI: a tutorial for junior neuro-imagers. Front Neurosci 8:1. http://dx.doi.org/10.3389/fnins.2014.00001




Percent signal change


## Statistical inference
 Carsten on prevalence test

 On statistical errors commonly made by neuroscientists:

 Erroneous analyses of interactions in neuroscienceLinks to an external site. http://www.nature.com/neuro/journal/v14/n9/full/nn.2886.html

 The statistical error that just keeps on comingLinks to an external site. http://www.theguardian.com/commentisfree/2011/sep/09/bad-science-research-error

 Study: A lot of mind and brain research depends on flawed statisticsLinks to an external site. http://bigthink.com/Mind-Matters/study-a-lot-of-mind-and-brain-research-depends-on-flawed-statistics

 On the interpretation of removable interactionsLinks to an external site. http://www.ejwagenmakers.com/2012/WagenmakersEtAl2012Loftus.pdf



## Correction for multiple comparisons
The following page explains the multiple comparison problem we face in neuroimaging and how random field theory is used to solve it.

http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesRandomFields

On the downside of using cluster level inferences, this paper (http://www.sciencedirect.com/science/article/pii/S1053811914000020)Links to an external site. has some interesting things to say.

Devlin JT, Poldrack RA (2007) In praise of tedious anatomy. NeuroImage 37:1033-1041. http://dx.doi.org/10.1016/j.neuroimage.2006.09.055


## Effect size and percent signal change
pdf of mumford paper
poster by camille maumet
cyril GLM paper
handbook of fmri data analysis

## Circularity

functional localizers

Kriegeskorte N, Simmons WK, Bellgowan PSF, Baker CI (2009) Circular analysis in systems neuroscience: The dangers of double dipping. Nat Neurosci 12:535-540. (along with supplemental material) http://dx.doi.org/10.1038/nn.2303

## Anatomical localization
importance of knowing where you are

Devlin JT, Poldrack RA (2007) In praise of tedious anatomy. NeuroImage 37:1033-1041. http://dx.doi.org/10.1016/j.neuroimage.2006.09.055


## Multivariate analysis
PCM paper


## High-resolution MRI
review by polimeni


## Free energy

## Computational



## Reporting

making figures
https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003833

Carp on reporting results

effect size maps (Cox: do we only care about p?)

A short article on to make better figures (with links to some matlab code): Data Visualization in the Neurosciences: Overcoming the Curse of Dimensionality (http://www.sciencedirect.com/science/article/pii/S089662731200428X.

This blog post has also some additional (http://practicalfmri.blogspot.co.uk/2012/07/methods-reporting-in-fmri-literature.html. interesting (http://practicalfmri.blogspot.co.uk/2012/10/draft-checklist-for-fmri-methods.html. suggestions.

An interesting paper that shows how little information is sometimes provided by authors : The secret lives of experiments: Methods reporting in the fMRI literature (http://www.sciencedirect.com/science/article/pii/S1053811912007057

better figures: Guillaume rousselet

COBIDAS

Poldrack RA, Fletcher PC, Henson RN, Worsley KJ, Brett M, Nichols TE (2008) Guidelines for reporting an fMRI study. NeuroImage 40:409-414. http://dx.doi.org/10.1016/j.neuroimage.2007.11.048

## Misc

Here are some articles and similar materials, mostly quite accessible, relating either to specific course content or addressing general issues within the neuroscience community.
