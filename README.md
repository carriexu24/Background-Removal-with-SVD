# Background-Removal-with-SVD

This project removes a still background from a video using Singular Value Decomposition (SVD).

First, we construct a matrix M from the video, where each column is a flattened image. Then we perform a full SVD on M and take the first rank to reconstruct the background image. The remaining part is the moving part in the video without background.

We also performed a randomized SVD by performing SVD on a smaller matrix that has approximately the same range as our original matrix. This method gives us acceptable results in a much shorter time compared to the full SVD.
