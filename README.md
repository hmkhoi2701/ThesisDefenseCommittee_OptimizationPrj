Table of contents:
- [Thesis Defense Committee Project Introduction](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj#thesis-defense-committee-project-introduction)
- [[For non-Vietnamese] Guides for reading input files](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj#for-non-vietnamese-guides-for-reading-input-files-eg-datatxt)
- [Collaborators](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj#collaborators)
- [To-do list / Features](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj#to-do-list--features)


# Thesis Defense Committee Project Introduction:
The link to the project: https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj/

A capstone project for the course Fundamentals of Optimization at Hanoi University of Science and Technology.  
The problem is fully stated in the file [ProjectProblem.pdf](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj/blob/main/ProjectProblem.pdf)

In short, there are N theses and M professors. They should be divided into K committees, with some requirements
   - Number of theses and professors in each committees should be bounded.
   - Every thesis should NOT be defended against its guiding professor
   - Similarity index between theses and professors in the same committees should exceed a certain value
We're going to execute an input file and return a solution that maximize the similarity index for all committees.

# [For non-Vietnamese] Guides for reading input files, e.g. [data.txt](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj/blob/main/data.txt)
1. The first line contains 3 elements, N (number of theses), M (number of professors), K (number of committees)
`10 6 3` means 10 thesis, 6 professors, 3 committees
2. The second line contains 6 elements, for example `3 4 2 3 8 8`, which can be seen in order:
    - Minimum and maximum number of thesis in a committee, `3 4` indicates min = 3, max = 4
    - Minimum and maximum number of professors in a committee, here they are `2 3`
    - Minimum similarity index of theses in the same committees, `8`
    - Minimum similarity index between theses and professors in the same committees, `8`
3. The next N lines is a NxN matrix, named s. The number at s[i][j] representing similarity index of thesis i and thesis j
4. The next M lines is a MxN matrix, named g. The number at g[i][j] representing similarity index of professor i and thesis j
5. The last line contains N elements, each representing which professor is in charge of which thesis  
In the file [data.txt](https://github.com/hmkhoi2701/ThesisDefenseCommittee_OptimizationPrj/blob/main/data.txt), `2 3 2 6 5 6 1 1 4 4` means professor 2 guided thesis 1, then they cannot be in the same committee; professor 3 guided thesis 2, professor 2 guided thesis 3 and so on... 

# Collaborators

# To-do list / Features
- [ ] Modelling the problem  
Choose 3-4 methods:
  - [ ] Linear Programming
  - [ ] Integer Programming
  - [ ] Constraint Programming
  - [ ] Heuristic method
- [ ] Generating random datasets
- [ ] Analyzing results, presentation

