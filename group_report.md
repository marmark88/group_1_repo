Daniel Felipe and Mark Cubi


AlphaFold Group Report


1. Biological problem the authors are trying to solve


The paper focuses on one of the central challenges in molecular biology, which is the long-time protein structure prediction problem: how to computationally predict accurate 3D protein structures from just sequence data. The importance of predicting a protein’s 3D shape wit$h high accuracy is that it would allow us to determine its biological function. Determining structures through experimental methods like X-ray crystallography and NMR spectroscopy can achieve this but these methods are slow and expensive, and not feasible at the scale of entire proteomes. Therefore, the central biological challenge is to reliably infer how a linear chain of amino acids folds into a precise 3D shape governed by physical interactions and evolutionary constraints. The AlphaFold system introduced in this paper uses a novel deep learning architecture that incorporates evolutionary, physical, and geometric information to predict protein structures with atomic accuracy.

The computational approach the authors use is neural networks to predict 3D coordinates of all heavy atoms for a given protein using the primary amino acid sequence. The network processes inputs through multiple layers of Evoformers and is then followed by the structure module that introduces an explicit 3D structure in the form of a rotation and translation for each residue of the protein. The Evoformer combines data from a related protein sequence and pairwise relationships between amino acids in the protein. The structure module serves as an end-to-end structure prediction that takes the previous output of the Evoformer and then directly predicts the full 3D structure of the protein.
