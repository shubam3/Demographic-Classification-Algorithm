# Age-and-Gender-Prediction
Using CNN algorithm and basic python language
We have trained data models to predict the gender and age of a person.
This is the Age and Gender prediction model built using Convolutional Neural Networks in Python. The model is built on the basis of Research Paper by Gil Levi and Tal Hassner. The neural architecture is built as written in the paper with slight modifications according to the dataset for better perfomance.

The dataset used are UTKFace Dataset and FairFace Dataset out of which Indian Race faces were seperated and the model was trained with.

Frameworks used
Tensorflow    pip install tensorflow
Numpy    pip install numpy
Keras    pip install keras
Pillow    pip install pillow
Performance of model
The output of the model consists of 2 classes for Gender Prediction, namely Male and Female and 9 classes for the Age Prediction, which are (0-3), (5-9), (10-19), (20-29), (30-39), (40-49), (50-59), (60-69), (70+). The table below shows the performance of model when tested on 13835 images containing Indian faces only.

 Male or Female represents what the model predicted. For eg: False Female means the model predicted Wrong and Prediction was Female. Which means actually it was Male.

Age Group	True Male	False Male	True Female	False Female
(0-2)	55	32	88	12
(3-9)	561	221	348	138
(10-19)	784	216	645	70
(20-29)	1701	222	1484	53
(30-39)	1157	166	1752	44
(40-49)	547	105	1062	26
(50-59)	382	88	645	22
(60-69)	96	56	249	6
(70+)	90	87	69	5
The Accuracy achieved in Gender Prediction is 78.3%

Below shown is the Confusion matrix of Age Prediction

Age Group	(0-3)	(5-9)	(10-19)	(20-29)	(30-39)	(40-49)	(50-59)	(60-69)	(70+)
(0-2)	175	8	1	3	0	0	0	0	0
(3-9)	267	1187	78	106	24	14	36	1	0
(10-19)	62	418	651	414	64	50	55	1	0
(20-29)	53	65	93	2539	338	264	107	1	0
(30-39)	38	38	42	942	1081	722	253	3	0
(40-49)	17	13	8	174	212	941	468	1	0
(50-59)	20	3	2	69	37	190	787	5	1
(60-69)	6	2	2	15	10	38	347	70	11
(70+)	12	0	1	4	2	9	110	19	35
The Accuracy achieved in Age Prediction is 53.96%(exact) and 86.72%(1-off).
