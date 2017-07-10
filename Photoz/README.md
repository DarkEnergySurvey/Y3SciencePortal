In this directory you will find products associated to Photoz Y3.

We have been validating with 2 different spectroscopic sample (We have created a basic point source removal to eliminate point sources from these catalogs (nopointsources)):

- A Y1like spectroscopic sample, same as the one used in Y1 analysis
- A smaller sample, trying to choose "the best" samples for Y1.

With this samples, we run through the science portal to train and validate: DNF, Lephare, TPZ, Annz2 and BPZ.
The sample is divided in a 60% for training, and 40% for validation purposes.
The validation sample is then weighted using the Lima procedure in order to get a sample representative of our data, for now, we are validating in:

- lssred: A similar sample to that one used in LSS BAO analysis, with cuts:  i<22.5   -1<gr<3.  -1<ri<2.5   -1<iz<2. and  
  (mag_auto_i - mag_auto_z) + 2.0*(mag_auto_r - mag_auto_i) > 1.7
  
- Y3main: Validating in a sample Y3 representative, cutting in: i<23.5 and -2<gr<4.  -2<ri<3.5   -2<iz<3.

In the directory you will find results for the Photo-z validation, as well as properties of the catalogs used, separately:

PROPERTIES

- properties_small_grizY_lssred_valid: Small spec sample, validating with grizY in lssred sample.
- properties_small_griz_lssred_valid: Small spec sample, validating with griz in lssred sample.
- properties_small_grizY_nopointsources_lssred_valid: Small spec sample, with pointsources removed, validating with grizY in lssred sample.
- properties_y1like_griz_lssred_valid: Y1like spec sample, validating with griz in lssredsample.

PROPERTIES COMPARISONS:

- Comparing small sample validation (grizY) with and without point sources. 
Look the ipynb in properties_small_grizY_nopointsources_lssred_valid versus properties_small_grizY_lssred_valid.
The biggest effect is seen in the plot magnitude versus redshift, how removing point sources actually removes a weird locus of bright objects at high redshifts and also in the color color plots, it can be seen a small locus that dissapears (stars? QSOs?). 

- Comparing small sample (grizY) versus (griz). Both without removing point sources.
Look the ipynb in properties_small_grizY_lssred_valid versus properties_small_griz_lssred_valid.
Nothing different.

- Comparing small sample (griz) versus Y1like (griz). Both without removing point sources.
Look the ipynb in properties_small_griz_lssred_valid versus properties_y1like_griz_lssred_valid.
In plot r-i r, none of them cover a region in r-i >1.5.
Nothing clearly different.


PHOTOZ VALIDATION

- dnf_small_griz_lssred_valid: DNF validation using small spec sample, using griz, validated in lssred.
- mlzlephannz2_small_griz_lssred_valid: Lephare, TPZ and Annz2 using small spec sample, using griz, validated in lssred.
- dnf_small_grizY_lssred_valid: DNF validation using small spec sample, using grizY, validated in lssred.
- dnf_small_grizY_lssred_valid_nopointsources: DNF validation using small spec sample, using grizY, removing pointsources, validated in lssred.
- dnf_y1like_griz_lssred_valid: DNF validation using Y1like spec sample, using griz, validated in lssred.


COMPARISON PHOTOZ VALIDATION

- Comparing griz versus grizY in DNF
Look ipynb in dnf_small_griz_lssred_valid versus dnf_small_grizY_lssred_valid.
Very little gain. 5bands have more 3sigma outliers at high redshift but it is uncertain if it is by lack of data, or other reason.
5bands seems to improve in sigma68, maybe, but not clear either.
4bands better bias?.

- Comparing griz DNF verdsus MLZ, Lephare and Annz2
Look ipynb in dnf_small_griz_lssred_valid versus mlzlephannz2_small_griz_lssred_valid.
Very similar results!!.

- Comparing grizY in DNF using small sample, with and without pointsources:
Look ipynb in dnf_small_grizY_lssred_valid versus dnf_small_grizY_lssred_valid_nopointsources.
nopointsources have better bias at high redshift and less outliers. Also a better Npoisson.
with pointsources we have high redshift better sigma68?.

- Comparing griz small sample versus Y1like (no point sources removed)
Look ipynb in dnf_small_griz_lssred_valid versus dnf_y1like_griz_lssred_valid.
Small one seems to have better metrics. Better Npoisson.

