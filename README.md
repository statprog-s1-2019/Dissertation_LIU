# Dissertation_LIU

The files is for the Experiment 1 - University of Edinburgh.

There are 4 data sets of Excel files and 3 Xpress mosel files are included.

## Data
Four different data sets are used to validate my models.

Each name of the InputDataFile includes the number of students, projects, and supervisors of this experiment inside the parentheses.

    InputDataFile1 = "MSc_1(89_115_46).xlsx"
    
    InputDataFile2 = "MSc_2(56_99_59).xlsx"
    
    InputDataFile3 = "MSc_3(90_124_43).xlsx"
    
    InputDataFile4 = "MSc_4(54_92_44).xlsx"

## Code
The mosel files are divided into two parts.

The first part is the mosel file "Model_0a_0b.mos", in which we can manually control the objective value to implement Model 0a or Model 0b. Besides, if the model 0a or 0b cannot obtain a feasible solution, Model 1a, 1b, 1c, 2a, 2b, 2c will automatically implement inside this mosel file.

The second part is the mosel file "Model_3a(combine_infeas).mos", "Model_3b(combine_infeas).mos", "Model_3c(combine_infeas).mos". If we cannot obtain a feasible solution by running "Model_0a_0b.mos" (i.e., None of Model 1a, 1b, 1c, 2a, 2b, 2c can generate a feasible solution), then Model 3a, 3b, 3c will be implemented.
