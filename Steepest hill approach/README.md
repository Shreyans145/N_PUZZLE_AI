
#  Steepest Hill approach


A variant of the simple hill-climbing algorithm is the Steepest Hill algorithm. This algorithm compares all of the present state's neighbouring nodes and chooses one neighbour node nearest to the target state. When it scans for multiple neighbours, this algorithm takes more time.

**Algorithm for Steepest-Ascent hill climbing**
1. Evaluate the initial state, if it is goal state then return success and stop, else make the current state as your initial state.
1. Loop until a solution is found or the current state does not change.
1. Let S be a state such that any successor of the current state will be better than it.
1. For each operator that applies to the current state;

    * Apply the new operator and generate a new state. 
    * Evaluate the new state.
    * If it is goal state, then return it and quit, else compare it to the S.
    * If it is better than S, then set new state as S.
    * If the S is better than the current state, then set the current state to S.

1. Exit.
