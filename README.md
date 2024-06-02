# Marigold
This project enhanced Marigold (a diffusion model for monocular depth estimation https://marigoldmonodepth.github.io/)
to estimate depth conditionally on multiple previous frames for videos. 
This program was intended to improved scale drift that is a pertinent problem in rotational SLAM (simultaneous localization and mapping)
We enhanced the model by applying different weights on the previous frames, combining the frames, and then
applying monocular depth estimation on the 'enhanced'combined frame. We tested multiple methods, 
specifically, averaging the previous frames, weighting the previous frames with exponential decay, 
using optimized weights, and a baseline method of using just the previous frame. We evaluated the methods using RSME by 
comparing them to ground-truth labels to the respective test images.

This code was developed with Hang Pham.
