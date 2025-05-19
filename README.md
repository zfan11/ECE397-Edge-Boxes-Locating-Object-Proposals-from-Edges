# ECE397-Edge-Boxes-Locating-Object-Proposals-from-Edges

This project implements a Python-based version of the EdgeBoxes object proposal algorithm.

Contents:
- Uses structured edge detection to extract edge maps.
- Groups edge pixels by orientation and connectivity.
- Filters weak or small edge groups.
- Builds an affinity graph between edge groups.
- Scores candidate bounding boxes based on group containment and boundary affinity.
- Supports random sampling and local refinement to find high-quality object proposals.

Usage:
1. Run the full pipeline in a Jupyter notebook or script:
2. Visualize results.

Dependencies:
- OpenCV (Only for structured edge detection, not for the algorithm)
- NumPy
- SciPy
- Matplotlib

Note:
Make sure to load a trained structured edge model (model.yml.gz) compatible with OpenCV's ximgproc.

Reference:
[1] C. L. Zitnick and P. Dollár, “Edge boxes: Locating object proposals from edges,” in *European Conference on Computer Vision (ECCV)*, 2014, pp. 391–405.
[2] P. Dollár and C. L. Zitnick, “Structured forests for fast edge detection,” in *IEEE International Conference on Computer Vision (ICCV)*, 2013, pp. 1841–1848.
