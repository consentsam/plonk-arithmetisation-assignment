# PLONK Arithmetisation Assignment

Calculate polynomials used in PLONK Arithmetisation. Fill in the values in this markdown to complete the assignment

The polynomial used in this assignment is: $$x^3 + x == 2$$

**Note: You can use the code from your `Lagrange Polynomial Assignment` to complete this**

## Gates

Complete the gates below, the first one is completed for you

### Gate 1

$$x_1 * x_1 = x_2$$

### Gate 2

$$x_2 * x_1 = x_3$$

### Gate 3

$$x_4 = 2$$

### Gate 4

$$x_3 * x_1 = x_4$$

## Assignments
Complete the assignment vectors, let $x_1 = 1$

$$\vec{a} = [1,1,2,1]$$

$$\vec{b} = [1,1,0,1]$$

$$\vec{c} = [1,1,0,2]$$

## Selectors

Fill in the below table for the values of $q_L$, $q_R$, $q_O$, $q_M$ and $q_C$, satisfying the equation: 

$$q_L * a + q_R * b + q_O * c + q_M * a*b + q_C = 0$$


|$q_L$|$q_R$|$q_O$|$q_M$|$q_C$|
|-----|-----|-----|-----|-----|
|  0  |  0 |  -1  |  1  |  0  |
|  0  |  0  | -1 |  1  |  0  |
|  1  |  0  |  0  |  0  |  -2  |
|  1  |  1  |  -1  |  0  |  0  |

## Domain

We will use the base field of $\mathbb{F_{17}}$ and the domain consisting of roots of unity

Fourth roots of unity in $\mathbb{F_{17}}$:
$$H: {1, 4, 16, 13}$$

## Cosets

$$k_1 = 2$$

$$k_2 = 3$$

$$k_{1}H: {2, 8, 15, 9}$$

$$k_{2}H: {3, 12, 14, 15}$$

## Interpolating Polynomials

$$f_a(x) = 4x^3 + 13x^2 + 4x + 14$$

$$f_b(x) = 13x^3 + 4x^2 + 13x + 5$$

$$f_c(x) = 12x^3 + 8x^2 + 14x + 1$$

$$q_{L}(x) = 3x^3 + 0x^2 + 5x + 9$$

$$q_{R}(x) = 16x^3 + 4x^2 + x + 13$$

$$q_{O}(x) = 4x^3 + 13x^2 + 4x + 12$$

$$q_{M}(x) = 14x^3  + 12x + 9$$

$$q_{c}(x) = 9x^3 + 8x^2 + 9x + 8$$

## Copy Constraints

| LHS | RHS | Domain of LHS | Domain of RHS |
|-----|-----|---------------|---------------|
|$a_1$|$b_1$|       1       |       2       |
|$a_2$|$c_1$|       4       |       3       |
|$a_3$|$a_3$|       16      |       16      |
|$a_4$|$b_2$|       13      |       8       |
|$b_1$|$b_2$|       2       |       8       |
|$b_2$|$b_1$|       8       |       2       |
|$b_3$|$b_3$|       15      |       15      |
|$b_4$|$c_2$|       9       |       12      |
|$c_1$|$a_2$|       3       |       4       |
|$c_2$|$b_4$|       12      |       9       |
|$c_3$|$c_4$|       14      |       15      |
|$c_4$|$c3$|       15      |       14      |

## Copy Constraints Polynomials

$$S{{\sigma}_1} = 6x^2 + 10x + 3$$

$$S{{\sigma}_2} = 15x^3 + 8x^2 + 2x + 5$$

$$S{{\sigma}_3} = 9x^3 + 15x^2 + 5x + 2$$

## Evaluation

-   Clone this repo.

    ```
    git clone https://github.com/DappCamp-Assignments/b12fdd542d4acb1d3d1772bcdea83edb96987c8048e05ff6eede9076a72af7fc
    ```

-   Create a new branch with your name. You can use the following command

    ```
    git checkout -b satyajeet-sindhiyani
    ```

-   Fill in the values in this file with your solution

-   Create a pull request from your branch to the main branch of the repo

-   Since this assignment is manually evaluated we will provide feedback on your solution in form of pull request comments
