---
layout: post
title: Image Preprocessing
---
### Methods
1. Normalization  
  * Normalize the image into range 0-1  
2. CLAHE(Contrast Limited Adaptive Histogram Equalization)
  * To remove artifacts in the tiles(8*8) which is the small block from origin image  
3. Gamma Correction  
  * nonlinear operation used to encode and decode luminace or tristimulus values in image  
  * V_out = A V_in^r  
  * if r < 1, it called encoding gamma or gamma compression, if r > 1, it is called decoding gamma or gamma expansion  
  * It is used to optimize the usage of bits( better for transformation)  
4. Crop out a certain thing
