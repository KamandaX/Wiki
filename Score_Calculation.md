# Score calculation
We can estimate the best suited phone by finding the average of answer multipliers for each aspect (specification). 
We then calculate the score by finding the product sum of multiplier averages and phone aspect scores.
The phone with the highest score is the one that gets recommended.

## Definitions:
* **A** - Set of answers
* **F** - Aspect
* **Af** - Answer multiplier for aspect f
* **n** - Aspect count
* **Mi** - Aspect multiplier sum
* **Pi** - Phone aspect score

## Formula
![M(A)=\frac{1}{|F|}\sum_{A\in F}A_{F}](https://render.githubusercontent.com/render/math?math=M(A)%3D%5Cfrac%7B1%7D%7B%7CF%7C%7D%5Csum_%7BA%5Cin%20F%7DA_%7BF%7D)

![Score = \sum_{i=0}^nM_i*P_i](https://render.githubusercontent.com/render/math?math=Score%20%3D%20%5Csum_%7Bi%3D0%7D%5EnM_i*P_i)
