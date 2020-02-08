# Video Synopsis-Key frames Selection based on a Distortion Minimization 


Matlab Code: https://www.mathworks.com/matlabcentral/fileexchange/46507-video-synopsis



This code is a simple implementation of the video
synopsis SEDIM and other methods (SEDIM-IN, CEA and TEA) proposed in [1].
The code is written by the authors of [1] (C. Panagiotakis, N. Ovsepian and E. Michael).
The main goal of the proposed method is to select from a video the most “significant” frames in order to broadcast, without apparent loss of content by decreasing the potential distortion criterion.
You can find more details in www.csd.uoc.gr/~cpanag
The initial videos and video synopsis results (with α = 0.1 and α = 0.3) of SeDiM, SeDiM-IN, CEA, TEA methods are given in https://www.dropbox.com/sh/rpysux4oa746jty/B265lHwpAB
https://www.dropbox.com/sh/rpysux4oa746jty/B265lHwpAB
Usage:

usage to run the method for foreman.avi with a= 0.1 (10%):

[KeyFr] = vsyn(0.1, 0, 'sum', 'foreman.avi');
It returns the key frames KeyFr (N x 4 array) of SEDIM, SEDIM-IN, CEA and
TEA methods [1], where N is the nuber of key frames. N is
determined by the first parameter (10% of total frames in this example).
Finally, it also writes the video synophis file for SEDIM (foreman_Video_Synopsis_a0.1.avi).

We will appreciate if you cite our paper in your work.

[1] C. Panagiotakis, N. Ovsepian and E. Michael, Video Synopsis based on a Sequential Distortion Minimization Method, International Conference on Computer Analysis of Images and Patterns, 2013.
