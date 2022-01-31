# BWSI Python Course Graded Assignments

These problems are ordered alphabetically, and *not* in order of ascending difficulty. Please consult the BWSI-EdX course page for the due dates for the respective problems.

## Installing the auto-grader

Complete [Module 1 of PLYI](https://www.pythonlikeyoumeanit.com/module_1.html) to install and configure Python on your computer, via Anaconda.

In order to run the auto-grader for these problems, you must install `bwsi_grader`. In your terminal, execute:

```shell
pip install bwsi_grader
```

This grader requires you to use Python 3.7 or later.


## Completing an Assignment

### 1. Open the Jupyter notebook for the problem of interest 

The coding problems are provided in Jupyter notebooks. Refer to [this section of PLYMI](https://www.pythonlikeyoumeanit.com/Module1_GettingStartedWithPython/Jupyter_Notebooks.html) for instructions for starting a Jupyter server, and for opening a Jupyter notebook.

Make sure that the conda environment from which you start the Jupyter server is also the one that you installed `bwsi-grader` in.


### 2. Read the problem description

At the top of the notebook will be a detailed description of the problem, as well as example that demonstrate how your function ought to behave. Read through this material carefully.

All of the problems here can be solved based on the materials presented in [PLYMI](https://www.pythonlikeyoumeanit.com/index.html). Please consult the appropriate sections of the website for guidance towards tackling any given problem. The website also has a search bar that you can utilitize.

Feel free to post questions on the course's piazza page.

### 3. Begin working on a solution

Below the problem description is the template for a function; you are responsible for filling out the body and return statement of that function. For some problems, you are also required to complete [the signature](https://www.pythonlikeyoumeanit.com/Module2_EssentialsOfPython/Functions.html#Arguments) for that function.

Whenever you make changes to that function, you must *execute the notebook cell containing the function's definition* in order for those changes to take effect.

### 4. Test your function

**Before you run the auto-grader, you should test your solution with some examples**. You will save a lot of time if you build an intuition for the solution that you are working on, and see if it behaves as you expect, before submitting your solution to the auto-grader.

Note that every problem gives you example use-cases for your function, complete with the input to the function and the expected output. These are ready-made test cases for you to use.
[Make a new cell in your Jupyter notebook](https://www.pythonlikeyoumeanit.com/Module1_GettingStartedWithPython/Jupyter_Notebooks.html#Familiarizing-Yourself-with-Jupyter-Notebooks) and try running your function yourself; do you see the output that you expect?

**Some Common Issues**

"My function doesn't return anything when I run it!"
- Did you include [a `return` statement](https://www.pythonlikeyoumeanit.com/Module2_EssentialsOfPython/Functions.html#The-return-Statement) in your function? If not, your function is returning `None`
- Is there an asterisk to the left of the cell where you are running your function? If so this means that your code is still running. Almost all of the solutions to these problems should run quickly (within a few seconds); if your code is running for a long time, there may be a while-loop in your code that is running forever. If this is the case, [kill your notebook's kernel](https://www.pythonlikeyoumeanit.com/Module1_GettingStartedWithPython/Jupyter_Notebooks.html#Familiarizing-Yourself-with-Jupyter-Notebooks) and inspect your function for while-loops that fail to end.


### 5. Submit your solution to the auto-grader

The notebook will contain a cell that imports a function from `bwsi_grader` and passes your solution to this. Running this cell will run your solution through the grader.

**You can run the grader as many times as you like**.

If there is a problem with your solution, the grader will try to print out a descriptive error message for what went wrong. It will also show you *how* your function was called by the grader, and what its expected behavior was; read this message carefully to understand how to fix your code.

If your solution is correct, the grader will print out a message saying so, and will print a hash code that you can submit on the BWSI Python course page, to prove that you completed the assignment.

**Some Common Issues**

"When I run the auto-grader cell I get an `ImportError` indicating that the module `bwsi_grader` cannot be found. 
 - Make sure that you installed `bwsi_grader` in the same conda environment from which you are running your Jupyter notebook.

"My function prints the correct solution when I run it, but the grader says that it returns `None`"
- Did you use a `print` statement in your code to print the answer, instead of a `return` statement to actually return the answer? This is likely the cause of this error.