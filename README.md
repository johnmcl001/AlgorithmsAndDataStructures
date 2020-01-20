# AlgorithmsAndDataStructures
This will follow chapters 1 to 10 of The Algorithm Design Manual by S.S. Skiena

# 1. Introduction to Algorithm Design 

1. An algorithm is a procedure that takes any of the possible input instances 
and transforms it to a desired output.

2. An algorithm has 3 properties, correctness, efficiency and ease of implementationj. 

## Robot Tour Optimization
1. __There is a fundamental difference between algorithms which always produce a 
correct result, and heuristics which may usually do a good job bu without
providing any guarantee.__

## Selecting the Right Jobs
1. Seeking counterexamples that break pretender algorithms in an important part
of the algorithm design process.

2. __Reasonable looking algorithms can easily be incorrect. Algorithm correctness
is a property that must be carefully demonstrated.__

## Reasoning about Correctness
1. Mathematical proofs consist of 4 parts:
    - Clear precise statement of what's to be proved
    - Set of assumptions of things which are taken to be true and used as part 
    of the proof
    - Chain of reasoning which leads from the assumptions to the statement to be
    proven
    - QED which denotes completed

### Expressing Algorithms 
1. The idea behind any algorithm must be clearly revealed when the algorithm is 
expressed, if this doesn't happen then the notation used is too low-level.

### Problems and Properties
1. Problem specifications have 2 parts:
    - Set of allowed input instances
    - Required properties of the algorithm's output
    
2. It is impossible to prove the correctness of an algorithm for a fuzzily
stated problem.

3. __An important and honorable technique in algorithm design is to narrow the 
set of allowable instances until there is a correct and efficient algorithm.__

4. Two common traps in specifying the output requirements of a problem:
    - Asking an ill-defined question
    - Creating compound goals (complicated goals)
    
### Demonstrating Incorrectness
1. The best way to prove that an algorithm is incorrect is produce an instance
in which it yields an incorrect answer. These are called counter examples.

2. Good counter example have 2 properties:
    - Verifiability: Calculate what answer your algorithm will give in an instance
    then display a better answer to prove that the algorithm didn't find it.
    - Simplicity: Make clear exactly why the proposed algorithm fails.
    
3. __Searching for counterexamples is the best way to disprove the correctness
of a heuristic.__

#### Techniques to Find Counter Examples

- Think small, easier to verify and reason about
- Think exhaustively
- Hunt for the weakness
- Go for a tie, provide instances where everything is the same size
- Seek extremes, many counter examples are mixtures of extremes

### Induction and Recursion
1. Recursion is mathematical induction. Both have general and boundary conditions:
    - The general condition breaks the problem into smaller and smaller pieces.
    - The boundary condition terminates the recursion.
    
2. Need to be aware of 2 types of errors when using induction:
    - Boundary errors
    - Cavalier extension claims, adding an extra item to a problem instance 
    might cause the optimal solution to change.
    
3. __Mathematical induction is usually the right way to verify the correctness
of a recursive or incremental insertion algorithm.__

### Summations
1. Concise expressions describing the addition of arbitrarily large sets of numbers.

2. 2 major classes of summation in algorithm analysis:
    - Arithmetic progressions
    - Geometric series
    
## Modeling the Problem
1. Formulating the application in terms of precisely described, well-understood problems

### Combinatorial Objects
1. Computing properties can be linked to certain words:
    - Permutations: arrangement, tour, ordering, sequence
    - Subsets:      cluster, collection, committee, group, packaging, selection
    - Trees:        hierarchy, dominance relationship, ancestor/descendant, taxonomy
    - Graphs:       network, circuit, web, relationship
    - Points:       sites, positions, data records, locations
    - Polygons:     shapes, regions, configurations, boundaries
    - Strings:      text, characters, patterns, labels
    
2. The act of modeling reduces the application to one of a small number of
existing problems and structures, this is inherently constraining and certain
details might not easily fit into the target problem.

3. Certain problems can be modeled in several different ways, some better than others.

4. __Modeling the application in terms of well-defined structures and algorithms
is the most important single step towards a solution.__

### Recursive Objects

1. Permutations, subsets, trees, graphs, points, polygons and strings can be 
thought of as recursive objects.

2. Recursive descriptions of objects require both decomposition rules and basis cases.
    - Basis cases are the specification of the smallest and simplest objects where 
    decomposition stops.



