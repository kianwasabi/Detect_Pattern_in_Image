# Detect Pattern In Image
CheckForPatternInImage.m is a simple Matlab script that detects a pattern (A) in an image (B) using the corr2 function.

## Idea:
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
The following flowchart briefly shows the structure of the Matlab script.<br>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221420977-b0ccaa78-8c78-4780-bd61-e4bc802faca7.png" height="auto" width="400"></a>

## Result: 
<ins>Case 1 - correct pattern recognition:</ins> <br>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/188312861-f0a08dee-336b-4419-89ff-6495b3b10457.png" height="auto" width="400" ></a>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221421492-b3102e71-e599-4bbc-81cb-331eab83e52f.png" height="auto" width="450" ></a>
<br>
<ins>Case 2 - correct pattern recognition with modified pattern:</ins> <br>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221421616-a05c0964-52d8-40b8-9add-39b51c49bc42.png" height="auto" width="400" ></a>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221422510-2e7a512f-b206-4cb9-a6d5-c9d28b02d92c.png" height="auto" width="450" ></a>
<br>
<ins>Case 3 - misleading pattern recognition:</ins> <br>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221421778-5aafafe1-6481-44a6-a0a0-26484743dd5d.png" height="auto" width="400" ></a>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221421808-2188f627-40fc-4e80-887f-fb57008ea85c.png" height="auto" width="450" ></a>
<br>
<ins>Case 4 - incorrect pattern recognition:</ins> <br>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221422027-c1bdbded-c8fe-4ff1-bbf5-a4c4d5829a24.png" height="auto" width="400" ></a>
<a href="url"><img src="https://user-images.githubusercontent.com/55065075/221422031-75081a1c-5a2c-4053-a471-7c45618d4288.png" height="auto" width="450" ></a>
<br>
<br></br>

## Project Status: 
Not perfect, but done.

## Built with:
Matlab - Required: Image Processing
