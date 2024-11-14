# Google-page-rank-algorithm
     DOCUMENTATION OF THE THE PAGERANK ALGORITHM: 

---Google's pagerank algorithm which rank's the websiites as per our search we are going to take a example search of 'Data science'.
If we take a 7 websites which are from A to G related to our search and we rank them based on the links on the webpage and suggest sequencily to the users there we use page rank algorithm if there are 7 blocks
which represents our webpages and have a hyperlinks in them so as  many hyperlink a webpage has we recommend it first to the user and same format applies till we suggest them all 7 webpages based on our number of hyperlink in an algorithm.

![image](https://github.com/user-attachments/assets/7ddce9f5-127f-4581-9b08-b75c6e6121ff)

As per this we can see importance of the webpage which recommends to the users based on the pagerank. As we can see most of the hyperlinks are situated or inserted in A webpage so if an user searched for 'Data science' then algorithm recommeds A webpage first on Google.

Indetail informaiton of page rank


Adjacency matrix
In the matrix below, you can see the links between pages:

$$
M = \begin{bmatrix}
   0 & 1 & 1 & 0 & 1 & 1 & 1 \\
   0 & 0 & 0 & 1 & 0 & 0 & 0 \\
   1 & 0 & 0 & 0 & 0 & 0 & 0 \\
   1 & 0 & 0 & 0 & 0 & 0 & 0 \\
   0 & 0 & 0 & 0 & 0 & 0 & 0 \\
   0 & 0 & 1 & 0 & 0 & 0 & 0 \\
   1 & 0 & 0 & 0 & 0 & 0 & 0 \\
\end{bmatrix}
$$

This matrix represents the structure.

where T2 is the total no of elements in the columns
 
AS per our links which are for A TO G just we have to keep in mind about incoming links and outgoing links with that we have to created the adjacency matrix from A-G webpages  where incoming links are noted in
the row and if we total all the elements in the rows then total will be the total incoming links in the specific webpages similarly if we add total elements in the  columns those will be the  total outgoing links
from a specific page as above. 

Similarly we create the transition matrix which show's the probability or percentage of the specifc webpages as follows

Transitional matrtix
In the matrix below, you can see probability of the links between pages:

$$
M = \begin{bmatrix}  
  0   &  1 & 1/2 & 0 & 1 & 1 & 1 \\                    
  0   &  0 &  0  & 1 & 0 & 0 & 0 \\
  1/3 &  0 &  0  & 0 & 0 & 0 & 0 \\
  1/3 &  0 &  0  & 0 & 0 & 0 & 0 \\
  0   &  0 &  0  & 0 & 0 & 0 & 0 \\
  0   &  0 & 1/2 & 0 & 0 & 0 & 0 \\
  1/3 &  0 &  0  & 0 & 0 & 0 & 0 \\
\end{bmatrix}
$$

Transation matrix is designed in a way if we add all of the elements in the columns then we will be getting 1:




