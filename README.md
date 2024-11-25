# Quantifying transconjugant
  This repository aims to detect cells on images obtained from fluorescent microscopy after conjugation has occurred between the donor cells and recipient cells. The images of the donors and recipients were captured in the mcherry and Cyan Fluorescent Protein (CFP) channel, respectively. The images were segmented using a machine learning tool 'Ilastik' into background and foreground (with imaged cells). The uploaded codes are excuted on these segmented images.
## counting.ipynb
first labels each centroid in foreground of the segmented images and counts them. 
## candidates.ipynb
labels each centroid in foreground of the segmented images and finds potential candidates of transconjugants. The candidate contains a donor cell (mcherry) and a recipient cell (CFP) that are closer to each other than the usual distance amongst the cells. The code also gives the coordinates of the potential candidates, such that their identities can be confirmed by eye.

