# nl-fol-translation


## Description
This repository is currently the home of my final project for Computational
Semantics at Brandeis University.

### Project Title: Translating Natural Language to First-Order Logic Using Hyperdimensional Embeddings and Constrained Decoding

### Professor: James Pustejovsky
### TA: Tim Obiso

### Description:

The primary objectives of this project are:
1. Establish a seq-to-seq baseline by fine-tuning an encoder-decoder 
transformer
2. Add constraints during decoding to help ensure the well-formedness of the
outputs
3. Add hyperdimensional embeddings of the FOL generations to rank candidate
generations, hopefully further refining FOL generation.

It is currently in a somewhat early stage. Evaluation is currently hindered by
ambiguity in predicate naming, and the baseline was fine-tuned without two FOL
operators.

The next steps are to:
1. Add the two missing FOL operators (⊕ and ↔) to the baseline
2. Rework evaluation to account for predicate ambiguity to have more useful
quantitative results
3. Add more rule-based constraints to the decoding process
4. Rework template-based HDV ranking to be more flexible and robust


## Instructions
1. Change the domain from 'github.com' to 'githubtocolab.com' in the URL of this
repository to open it in Google Colab.
2. Set the runtime to GPU.
3. Run the cells in the notebook `fol_translation.ipynb` (in-order) to create the 
HDV embeddings and save the variables collected from the dataset before running
the experiments.
