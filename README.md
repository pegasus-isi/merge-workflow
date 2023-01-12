# Merge Workflow 

# Dependencies
- Pegasus v5.0+
- Python 3.6+

![Merge](https://user-images.githubusercontent.com/36110304/210929333-d5c9b20a-912a-43c1-8aef-66dcd8a76636.png)

# File Description

<b>plan.sh:</b> Consists of all commands to be executed to run the workflow. Takes care of planning the pegasus workflow and initialising where the input files are and where output files should be located after execution of workflow. 

<b>workflow_generator.py:</b> Creates the abstract workflow, the replica catalog, the transformation catalog, and the site catalog. It has a job: Cat which is used to invoke the executables present in the bin folder.

# How to run the workflow?
```
# Plan and run the workflow generator to create an abstract workflow for the given input files
./workflow_generator.py   # Generate the workflow.yaml file
./plan.sh workflow.yaml
```
