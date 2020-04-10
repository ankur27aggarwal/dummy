# Abstract 

Code cloning refers to similar or identical fragments of code.Reusing existing code for increasing software productivity is a key element of object oriented programming which makes code clone detection and management a primary concern for the current industry. Consequently, this cloning process may lead to bug propagation that significantly affects the maintenance cost. By considering this problem,detecting code clones  appears as an active area of research. For our project we  used machine learning and similarity search  to detect the similarity between the two code segments on the basis of lexical analysis of programs. We have used K-Means algorithm (to group the similar code in same cluster) and Locality Sensitive Hashing(LSH to find the similar code fragments) to find similar codes

# 1. Introduction

Code clones are fragments of codes which are identical to each other, these clones are generated using copy and paste activities of the programmer, but the main problem with code clones is replication of bugs and difficulties in software comprehension and maintenance, so it becomes imperative to detect these clones. The 4 types of clones are:

- Exact clones (Type 1): Identical code segments except for changes in comments, layouts and whitespaces. 

- Renamed clones (Type 2): Code segments which are syntactically or structurally similar other than changes in comments, identifiers, types, literals, and layouts. These clones are also called parameterised clones. 

- Near Miss clones (Type 3): Copied pieces with further modification such as addition or removal of statements and changes in whitespaces, identifiers, layouts, comments, and types but outcomes are similar. These clones are also known as gapped clones. 

- Semantic clones (Type 4): More than one code segments that are functionally similar but implemented by different syntactic variants

The aim of our project is to detect type 1 and type 2 clones. As, most of the programmers try to simply replicate their previous work and reuse existing pieces of code, due to this trend many bugs are introduced in the software unknowingly which are very hard to detect once the program reaches a certain level of complexity.With our approach of using machine learning we want to detect the clones in such a way that it can be used  for various other purpose also like :- aspect mining, programunderstanding, plagiarism detection, copyright infringement investigation, code compaction, software evolution analysis, code quality analysis, bug detection and virus detection may need the extraction of semantically or syntactically similar code blocks, making clone detection effective and useful part of software analysis. 

# 2. Methods and Methodology 

It further is divided into the phases that are :- 

- Data generation 
- algorithm implementation

# 2.1  Data Preparation

There was no available dataset for code clones,so there were no definitive set of features to characterize  these code clones.Therefore we chose the IJADataset which is a collection of java programs and contains 47k files with around 10092k lines of code. 

We performed the following set of operations to generate data suitable for algorithms.
- Step 1 :- Injection of code clones in dataset .
###
- Injecting Type 1 clones(Exact CLones)-Created multiple copies of the codes,Addition of comments in few codes.
- Injecting Type 2 clones(Renamed CLones):Modifications in identifier names including Type 1 changes














