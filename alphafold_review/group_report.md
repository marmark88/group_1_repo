Daniel Felipe and Mark Cubi


AlphaFold Group Report


1. Biological problem the authors are trying to solve

The paper focuses on one of the central challenges in molecular biology, which is the long-time protein structure prediction problem: how to computationally predict accurate 3D protein structures from just sequence data. The importance of predicting a protein’s 3D shape wit$h high accuracy is that it would allow us to determine its biological function. Determining structures through experimental methods like X-ray crystallography and NMR spectroscopy can achieve this but these methods are slow and expensive, and not feasible at the scale of entire proteomes. Therefore, the central biological challenge is to reliably infer how a linear chain of amino acids folds into a precise 3D shape governed by physical interactions and evolutionary constraints. The AlphaFold system introduced in this paper uses a novel deep learning architecture that incorporates evolutionary, physical, and geometric information to predict protein structures with atomic accuracy.

2. The computation approach the authors are proposing to use

The computational approach the authors use is neural networks to predict 3D coordinates of all heavy atoms for a given protein using the primary amino acid sequence. The network processes inputs through multiple layers of Evoformers and is then followed by the structure module that introduces an explicit 3D structure in the form of a rotation and translation for each residue of the protein. The Evoformer combines data from a related protein sequence and pairwise relationships between amino acids in the protein. The structure module serves as an end-to-end structure prediction that takes the previous output of the Evoformer and then directly predicts the full 3D structure of the protein.

3. The most important references the paper relies on

The AlphaFold paper builds heavily on prior work in three main areas: evolutionary biology, structural bioinformatics, and deep learning techniques in structural biology. Foundational concepts include the use of multiple sequence alignments (MSAs) to extract evolutionary couplings between residues, drawing on earlier methods such as Direct Coupling Analysis (DCA) that showed correlated mutations encode structural proximity. It also relies on decades of protein structure databases, particularly the Protein Data Bank (PDB), which provides the experimental structures used for training and evaluation. From the machine-learning side, the work is deeply influenced by mechanisms and architecture originally developed for natural language processing. Finally, the CASP (Critical Assessment of Structure Prediction) experiments are a key reference framework, providing standardized benchmarks that shaped both the evaluation methodology and the historical context in which AlphaFold’s advance is measured.

4. Reasons why you will not be able to replicate the study's findings using their GitHub repository

The main reason we would not be able to replicate the results is due to hardware limitations on a typical pc. AlphaFold was developed and run using advanced GPUs capable of handling extremely large computational workloads. Attempting to perform the same computations on a standard pc would be impractical or impossible. In addition, the datasets required by AlphaFold are extremely large and exceed the available memory on most personal machines, making it difficult to load and process them efficiently. The AlphaFold GitHub repository primarily provides a pre-trained model, meaning that users are not reproducing the full training process. Re-training the model from scratch would not be feasible on a personal computer and would encounter the same computational and memory constraints described above. A smaller issue we would run into is having to download all the packages and the exact versions they used in the study.


