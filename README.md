# Pipeline
a) Get a grayscale image - that enables us to process differently colored lane lines similarly  
b) Blur the image to reduce noise  
c) Use canny algorithm to extract edges  
d) Use Hough transform to select distinct and useful lines  
e) Apply heuristics to weed out some unnecessary edges  
f) Merge directionally similar but sometimes diverging lines to propose lane lines  
g) Smoothen changes in lane lines over time by taking a moving average of recent past lane lines  

# Shortcomings
a) All parameters are currently heuristically determined  
b) All lane lines are straight  
c) Region of interest is near-statically determined and does not account for many real-life considerations  

# Possible Improvements
a) Heuristics and parameters (for image processing/CV algorithms) can be improved via deeper experience with vision  
b) Many parameters can be machine-learnt via examples  
c) Moving averages, line merging schemes can be adaptive in nature  
d) Many specific improvements are in code-comments  
