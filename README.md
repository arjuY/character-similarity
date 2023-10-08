# Vector Space Semantics for Similarity between Eastenders Characters
In this project, a vector representation of a document containing lines spoken by a character in the Eastenders script data is created then improved such that each character vector is maximially distinguished from the other character documents. This distinction is measured by how well a simple information retrieval classification method can select documents from validation and test data as belonging to the correct class of document (i.e. deciding which character spoke the lines by measuring the similarity of those character document vectors to those built in training).

# Dataset
This data is not publicly avalilable. The following columns from the eastenders's dataset are used for this project: Episode, Scene, Scene_info, Character_name, Line. As the lines of each character are not evenly distributed in terms of frequency, the first **360 lines** of each character in the training data is used to create the training documents, and the first **40 lines** in the test data.

# Part A
## Preprocessing
It is done by using various techniques and the performance was measured individually for each technique and combinations of the techniques based on mean rank, accuracy and cosine similarity. The combination of technique that gave good results are removing punctuation, stopword removal and lemmatization.
## 
