# Background-Removal-with-SVD
This project removes a still background from a video using truncated SVD.

First, we construct a matrix M from the video, where each column is a flattened image. Then we perform SVD on M and take the first rank to reconstruct the background image. The remaining part is the moving part in the video without background.
