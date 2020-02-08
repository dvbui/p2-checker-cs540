# p2-checker-cs540

## How to Use
- Clone this GitHub repository to a Linux machine (such as your CS lab computer)
- Create a file named ```input.txt``` in the same folder with ```checker_p2.pyc```
- Copy and paste the solution path to ```input.txt```. Do not include the ```Max queue length``` line.
- In the directory of ```checker_p2.pyc```, run ```python -i checker_p2.pyc``` (this code is written in Python 2)
- Call ```check("input.txt")```
- If the solution path is valid, the last output line will be ```Accepted```. If the solution path is invalid, the last three output lines would be ```Wrong answer on step i``` with step ```i``` be the transition from the ```i-th``` state to the ```i+1-th``` state, and these two states.

## Note
- I did not fully check the correctness of this checker. Use it at your own risk.
- This checker only checks the validity of the path. It does not check the optimality or the correctness of the heuristic function.
- Do not decompile this code and use it in your program. (To avoid plagiarism, I decided to not generate successor states to check whether the new states are valid. I will also publish my code after the deadline of the assignment).

## Example
```
ssh <your-cs-username>@best-linux.cs.wisc.edu
Input your password
cd Documents
git clone https://github.com/dvbui/p2-checker-cs540
cd p2-checker-cs540
vim input.txt
(paste the solution path, without the Max queue length line
(save the input.txt file)
python -i checker_p2.pyc
>>> check("input.txt")
...
Accepted
(or)
Wrong answer on step 1
[State 1]
[State 2]
```
