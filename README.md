# Detect Pattern In Image

The "corr2" function in matlab (R = corr2(A,B)) proves to be very useful for pattern recognition in image processing. <br>
This function can be used to analyze two 2-dimensional images of the same size based on their similarity. <br>
First, both images need to be converted to 𝑛 𝑥 𝑚 -sized arrays. 
It should be noted that the arrays must be of the same dimension in order to be processed further. <br>
With the parameters (A) and (B) passed to the "corr2(..,..)" function, the correlation coefficient R is returned as result. 
The correlation coefficient R represents the similarity between (A) and (B) by setting the relation of the respective pixel intensity in relation to the average pixel intensity of the whole image. 
<br>
Hence, the corr2 function represents the following equation to determine the correlation coefficient R:
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221416447-87b7693e-89d1-4df1-8137-5b65d3d09341.png" height="auto" width="300"></a>
<br>
According to the equation R lies between 0 and 1; Where R = 0 means that there is no correlation and R = 1 indicates the maximum strengthof the relationship.<br></br>
(see: <a href="https://www.mathworks.com/help/images/ref/corr2.html">[1]</a> & <a href="https://stackoverflow.com/questions/27343283/explaining-corr2-function-in-matlab">[2]</a>)

## Concept:
First, the script converts the imported image (A) and pattern (B) from RGB to GRAY-scale images. 
Second, it is checked whether image (A) is larger or at least quals the size of pattern (B).
If the size check of (A) and (B) results in a
At the end, a red rectangle is placed at the  and the correlation coefficient (R) is displayed in the command window.

## Result: 
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/188312861-f0a08dee-336b-4419-89ff-6495b3b10457.png" height="auto" width="400" ></a>
<br></br>
In Matlab the Corr2 function computes the 2D correlation coefficient (R) between two Images.
CheckForPatternInImage.m is a simple Matlab script that detects a pattern (A) in an image (B) using the corr2 function.

## Project Status: 
Done.

## Built with:
Matlab - Required: Image Processing Toolbox

## Author:
Kian David Warias

