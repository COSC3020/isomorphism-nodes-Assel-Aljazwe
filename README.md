[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# Proof:

To prove that two graphs $A$ and $B$ cannot be isomorphic if they do not have the same number of nodes, we can utilize the formal definition of isomorphism and approach this through proof by contradiction.

## Formal Definition of Isomorphism

Two graphs $G_1=(V_1, E_1)$ and $G_2=(V_2, E_2)$ are isomorphic if there exists a bijection $f: V_1 \rightarrow V_2$ such that for any pair of vertices $(u,v) \in E_1$, it is true that $(f(u),f(v)) \in E_2$, and vice versa.

## Proof by Contradiction

### Assumption

Assume, for the sake of contradiction, that two graphs $G_1$ and $G_2$ are isomorphic despite $G_1$ having a different number of nodes than $G_2$, say $|V_1| \neq |V_2|$ where $|V_1|$ and $|V_2|$ represent the number of elements of the vertex sets of $G_1$ and $G_2$, respectively.

### Contradiction

- **Bijection Requirement**: For two graphs to be isomorphic, there must be a one-to-one and onto function (bijection) between their vertex sets. A bijection means every element of one set is paired with exactly one element of the other set, and every element of the second set is paired with exactly one element of the first set.

- **Implication of Different Number of Nodes**: If $|V_1| \neq |V_2|$, it is impossible to establish a bijection between $V_1$ and $V_2$ because there would either be elements in $V_1$ without a counterpart in $V_2$ or vice versa. This violates the fundamental requirement for a bijection, because a one-to-one correspondence between all elements of both sets cannot be achieved.

- **Why This Doesn't Work for Isomorphism**: This inability to establish a bijection directly contradicts the requirement for isomorphism. Thus, the initial assumption that $G_1$ and $G_2$ can be isomorphic despite having different numbers of nodes is false.

## Conclusion

The contradiction shows that for two graphs to be isomorphic, they must have the same number of nodes. This is because isomorphism requires a bijection between the vertex sets of the two graphs, which is only possible if the sets have an equal number of elements. Therefore, if two graphs do not have the same number of nodes, they cannot be isomorphic.
