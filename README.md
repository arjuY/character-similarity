# Vector Space Semantics for Similarity between Eastenders Characters
In this project, a vector representation of a document containing lines spoken by a character in the Eastenders script data is created then improved such that each character vector is maximially distinguished from the other character documents. This distinction is measured by how well a simple information retrieval classification method can select documents from validation and test data as belonging to the correct class of document (i.e. deciding which character spoke the lines by measuring the similarity of those character document vectors to those built in training).

# Dataset
This data is not publicly avalilable. The following columns from the eastenders's dataset are used for this project: Episode, Scene, Scene_info, Character_name, Line. As the lines of each character are not evenly distributed in terms of frequency, the first **360 lines** of each character in the training data is used to create the training documents, and the first **40 lines** in the test data.

# Part A
**Preprocessing, Feature Extraction and Error Analysis**
Proprecessing and Feature extraction is done by using various techniques and the performance was measured individually for each technique and combinations of the techniques based on mean rank, accuracy and cosine similarity. Error analysis is done to find out the extra feature that can be used to create a better vector representation.

# Part B
**Added dialogue context and scene feature, improved vectorization method**
The Scene_info column is used to add scene feature and Lines before and after a particutar Line are take for the dialogue context. A matrix transformation technique called TF-IDF is used. TF-IDF scales down the impact of tokens that occur very frequently in the corpus making it a common term weighting scheme in information retrieval.

The final mean rank acheived on test data is 1.375
