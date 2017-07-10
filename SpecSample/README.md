#SPECSAMPLE

In this directory you will find products associated to Training set maker in the Science Portal, including the parent Spectroscopic sample before it has been matched to Y3

We have created 2 validation samples based on different spectroscopic sample: 

- A Y1like spectroscopic sample, same as the one used in Y1 analysis (in y1like_spec directory)
- A smaller sample, trying to choose "the best" samples for Y1.      (in small_spec directory)

We then match to Y3A2, for sources within -2<gr<4.  -2<ri<3.5   -2<iz<3.  Matching within 1 arcsecond to the spectroscopic catalog.
We create 2 version of each one, once where we remove point sources, and the other without:

- Y1 like spectroscopic sample matched to Y3A2  (y1like_spec_Y3 directory)
- Y1 like spectroscopic sample matched to Y3A2 with point sources removed (y1like_spec_Y3_nopointsources directory)
- Small sample spectroscopic sample matched to Y3A2 (small_spec_Y3 directory)
- Small sample spectroscopic sample matched to Y3A2 with point sources removed (small_spec_Y3_nopointsources directory)


With this samples, we run through the science portal to train and validate: DNF, Lephare, TPZ, Annz2 and BPZ..

