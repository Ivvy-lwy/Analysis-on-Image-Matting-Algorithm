# Analysis of Autonomous Image Matting Algorithms: SHM vs. GFM

## Description
In the realms of deep learning and computer vision, image matting stands out as a prominent technique for the discerning extraction of foregrounds from varied backgrounds. Traditionally, most image matting methodologies necessitate user-generated trimaps to tackle intricate regions like hair, a step that often becomes a bottleneck for automation.

This project delves into a comparative analysis between two deep learning algorithms—Semantic Human Matting (SHM) and Glance and Focus Matting Network (GFM)—that have been developed to transcend this limitation. These algorithms are exemplary in their ability to autonomously learn semantic information directly from RGB images, thereby generating high-quality alpha mattes without necessitating human interaction.


## Dataset Utilized
* P3M-10k:
  A comprehensive portrait image dataset instrumental for the reproduction of experimental results and sensitivity analysis.
* AM-2K:
  A natural animal dataset employed to assess the models’ generalization capabilities and performance on unexplored domains.
