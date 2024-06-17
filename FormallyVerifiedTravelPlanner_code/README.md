This code packages are for reviewers’ checking only. Please do not distribute to others. We will release the codes and results after the review.
We test our methods with the tasks developed by previous researchers, which are all open to use for common research. Our research is consistent with their intended use.

## Setup Environment

1. Create a conda environment and install dependency:
```bash
conda create -n fmtravelplanner python=3.9
conda activate fmtravelplanner
pip install -r requirements.txt
```

2. The UnsatChristmas dataset is provided in `database_small` folder. You can run interactive plan repair experiment with this database.

3. To run satisfiable plan generation experiment, refer to paper "TravelPlanner: A Benchmark for Real-World Planning with Language Agents" and their github repo to download their database and train/validation/test set.

## Running
1. Run test_travelplanner.py for satisfiable plan generation experiment. The command is ```python test_travelplanner.py  --set_type $SET_TYPE --model_name $MODEL_NAME```
2. Run test_travelplanner_interactive.py for unsatisfiable interactive plan repair experiment for TravelPlanner. Follow the instructions in file to first collect initial codes and then do the plan repair. 
3. Run test_unsat.py for unsatisfiable interactive plan repair experiment for UnsatChristmas. Follow the instructions in file to first collect initial codes and then do the plan repair. 

## Note
Run ```export OPENAI_API_KEY=YOUR_OPENAI_KEY``` to set up your openai key.