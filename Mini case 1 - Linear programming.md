QUESTIONS

1. What are the two parameters that the LpProblem function implements?

Beef and Chicken percent 

2. Is it mandatory to name the prob variable as prob?

Is not mandatory to name it “prob” it´s ok to choose any valid variable name, but for the context it is a good choice to name it prob to easily identify and indicate the purpose or content of the variable.

3. What are LpContinous and LpInteger used for?

Lp Continuous → variable type indicates that a decision variable can be any real number within a specified range. These variables can take fractional values, and the LP solver can search for the optimal solution within the continuous space.

LpInteger → variable type is used to specify that a decision variable must be an integer. This restriction allows for more flexibility in modeling real-world problems where certain quantities or decisions are inherently discrete.

4. Explain and copy the section of code that defines the objective function.

![image](https://github.com/naomigonzalez1/My_repo/assets/133794721/b46e7e4a-f0a0-4f2c-a88b-eb30ad1bd526)

The objective function has two variables x1 and x2. The coefficients 0.013 and 0.008 represent the cost of ingredients per unit of x1 (ChickenPercent) and x2 (BeefPercent), respectively. The sum of these two terms represents the total cost of ingredients per can. The second argument "Total Cost of Ingredients per can" helps in identifying the objective function when printing or analyzing the problem later.

5. Explain and copy the section of code that defines the constraints.

![image](https://github.com/naomigonzalez1/My_repo/assets/133794721/f011cb03-0660-4267-8e61-f650ddf35a01)

In this case, the constraints are the symbols <= / >= in the code, because it asks that the values have to be more than or less than 8.0, 6.0, 2.0 and 4.0 to get us the percentage for protein, fat, fiber and salt.

6. Is this a minimization or maximization problem? 

This is a minimization problem because they seek to reduce the cost of
  production of cat food.
  
7. Run the WhiskasModel1.py code. (no need to make changes, just run it as is) What is the value of the following variables? 
![image](https://github.com/naomigonzalez1/My_repo/assets/133794721/13a02f38-5a79-4a07-b27a-3af007472bad)


Status: Optimal
Beef Percent = 66.0
ChickenPercent = 34.0
Total Cost of Ingredients per can = 0.97
