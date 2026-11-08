# shortest-holonomy-loops
How short can a loop of complex subspaces be if parallel transport must produce a prescribed rotation? This proof solves Montgomery’s isoholonomic problem for complex Grassmannians in every positive codimension, with an exact length formula and an explicit shortest loop.

# The Shortest Loop with Prescribed Holonomy

Imagine carrying an arrow around a triangle on a globe, keeping it parallel as you move. When you return to the starting point, the arrow can point in a different direction. That change is called **holonomy**.

This proof asks a version of that question for complex subspaces. Move a subspace around a loop while carrying an orthonormal frame along with it. The subspace returns to where it started, and its frame can come back rotated. **If we specify the final rotation in advance, how short can the loop be?**

The proof gives the exact shortest length and constructs a loop that achieves it. The answer depends on the rotation’s eigenphases and on how many **auxiliary dimensions**, or directions outside the starting subspace, are available. The previously published lower bound is attained exactly when there is at least one auxiliary dimension for each nonzero eigenphase, counted with multiplicity. [Sönnerborn’s 2024 paper](https://doi.org/10.1103/PhysRevA.109.062433)

## The proof in plain English

1. **Find the cost of sharing a direction.** A shortest loop can be described by matrices. The condition that the subspace returns to its starting point forces integer-spaced spectral data. An eigenvalue ordering rule called *interlacing* lets us split that data into groups, one per auxiliary direction. It gives a lower bound on the squared length. Each phase has its own cost, and two phases in the same group add a penalty.

2. **Spread the phases out.** Mark the phases on a line and give each auxiliary direction a color. The penalty for two marks of the same color can be calculated from the intervals that contain both. In any interval, the fewest same-color pairs occur when the colors are as evenly represented as possible. Sorting the phases and cycling through the colors balances **every interval at once**. This is why the round-robin assignment minimizes the total penalty.

3. **Build a loop that reaches the bound.** The proof writes down an explicit motion for each group using one auxiliary direction. The motions run simultaneously in orthogonal subspaces, so their squared speeds add. The resulting loop produces the prescribed rotation at exactly the length forced by the lower bound.

For example, with phases of \(3/4\), \(1/2\), and \(1/4\) of a turn and two auxiliary dimensions, the shortest construction groups \(3/4\) and \(1/4\) together and gives \(1/2\) its own direction. The proof explains both why this arrangement wins and how to realize it as an actual loop.
