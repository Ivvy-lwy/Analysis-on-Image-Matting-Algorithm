# Analysis of Autonomous Image Matting Algorithms: SHM vs. GFM

## Overview
This project is part of the University of Toronto CSC413 Neural Networks & Deep Learning coursework. It focuses on leveraging machine learning algorithms to predict the likelihood of students correctly answering specific diagnostic questions in an online education setting. The predictions are based on the students' prior responses to other questions and the responses from other students.

## Description
In the realms of deep learning and computer vision, image matting stands out as a prominent technique for the discerning extraction of foregrounds from varied backgrounds. Traditionally, most image matting methodologies necessitate user-generated trimaps to tackle intricate regions like hair, a step that often becomes a bottleneck for automation.

This project delves into a comparative analysis between two deep learning algorithms—Semantic Human Matting (SHM) and Glance and Focus Matting Network (GFM)—that have been developed to transcend this limitation. These algorithms are exemplary in their ability to autonomously learn semantic information directly from RGB images, thereby generating high-quality alpha mattes without necessitating human interaction.

Read the complete report [here](https://github.com/Ivvy-lwy/Analysis-on-Image-Matting-Algorithm/blob/main/csc413-team%2090-project%20report.pdf).

## Method / Algorithm
### Semantic Human Matting (SHM)
SHM captures semantic information and matting details using T-net to extract semantic information and M-net to generate a new alpha matte. The fusion module then produces the final alpha matte.

### Glance and Focus Matting (GFM)
GFM consists of a shared encoder and two separate decoders to learn both tasks in a collaborative manner for end-to-end image matting. The predictions from glance and focus decoders are merged with a collaborative matting module (CM).

## Sensitivity Analysis on Image Preprocessing
The project investigates the effects of image preprocessing, such as resizing, random cropping, and rotations, on the performance of the algorithms. The analysis includes the impact of patch size and the trade-off between performance and running time.

## Extended Work
The models were tested on 200 images from the AM dataset to investigate their generalization to other datasets. The results show a domain gap between portrait and animal images.

## Conclusion
The report provides insights into two deep learning image matting algorithms and their performance with different preprocessing settings. The findings can be beneficial for applications where extracting semantic information is crucial.

## References
1. Chen, Q., Ge, T., Xu, Y., Zhang, Z., Yang, X., & Gai, K. (2018). Semantic human matting. In Proceedings of the 26th ACM international conference on Multimedia (pp. 618-626).
2. Sengupta, S., Jayaram, V., Curless, B., Seitz, S. M., & Kemelmacher-Shlizerman, I. (2020). Background matting: The world is your green screen. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (pp. 2291-2300).
3. Li, J., Zhang, J., Maybank, S. J., & Tao, D. (2022). Bridging composite and real: towards end-to-end deep image matting. International Journal of Computer Vision, 1-21.
4. Li, J., Ma, S., Zhang, J., & Tao, D. (2021). Privacy-preserving portrait matting. In Proceedings of the 29th ACM International Conference on Multimedia (pp. 3501-3509).
