# OCR
Repository for an Optical Character Recognition SW specifically tailored for formulae, thought to enable blind and visually impaired students to autonomously approach advanced mathematical classes and courses.

# Credits
Developed and maintained from Giuseppe Airò Farulla (mailto: giuseppe.airofarulla@polito.it), Nadir Murru, Rosaria Rossini.
Property and copyright 2015-2016 Politecnico di Torino, Università degli Studi di Torino, CINI.

# Datasets
To fair compare performances and results obtained from different authors in the critical field of characters segmentation we propose two datasets described as follows.
Both datasets are made publicly available free of charge to the community of researchers, under the GNU General Public License Version 3, in the hope that they will foster more rigorous comparison works and analysis 

The first dataset, hereby called dataset A, contains images of handwritten cursive characters we have built relying on samples from the CCC dataset. The CCC database contains samples of cursive characters that were manually extracted from images coming from different input sources, mainly related to American Post Services. They include both upper and lower case letters. Each sample is stored as a binary matrix within the database, and accompanied with information about the size of the matrix itself and the character that is represented.
Starting from the whole database, we developed randomly extracted some samples, taking care of maintaining a uniform distribution for all the characters chosen, both in their upper and lower version.
These samples were later combined and merged together to form two, three, and four touching character patterns, each of whom is accompanied by a textual descriptor indicating the index of the proper cut column (or columns, in the case of three and four multiple touching character patterns).
Dataset A contains 153 images, of which 139 represent two touching character patterns, and the other are equally divided into three and four touching character patterns.
Dataset A is organized as a collection of three subfolders, for 2, 3 or 4 touching characters: each image (PNG file) is accompanied from a descriptor (TXT file) with the same integer identifier; please note that identifier are repeated among the 3 folders (starting from 1).

The second dataset, in the following called dataset B, contains images of sided machine printed characters. 
We have identified a list of six font types (namely Cambria, Candara, Georgia, Lucida Sans Regular, Times New Roman and Verdana Bold) and three sizes (namely 10, 20 and 25); for each type and size we have combined into images the lower characters from the alphabet to form two, three, and four touching character patterns. Each image filename acts as a descriptor, which indicates the characters represented in the image itself as they should be recognized from an OCR software.
Dataset B contains 189 images (where 168 represent two touching characters).
Dataset B is organized as a collection of three subfolders, for 2, 3 or 4 touching characters: each image (PNG file) has a name of the form as "list of characters_font name".