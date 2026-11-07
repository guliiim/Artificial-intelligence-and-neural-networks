# Early prediction of student risk from weekly clickstream (OULAD)

Final project, AI and Neural Networks. Thesis: An Intelligent System for Predicting Students' Learning Activity
in Educational Platforms Using Big Data Technologies.

## Run
1. `pip install -r requirements.txt`
2. Open `final_project.ipynb` and run all cells. OULAD (CC BY 4.0) is downloaded automatically into `data/oulad/`
   (or download it from https://analyse.kmi.open.ac.uk/open_dataset and put the csv files there).
   Set the environment variable `QUICK_RUN=1` for a fast test run.
3. Score new students: `python inference.py models_saved/sample_input.csv predictions.csv`

## Files
- `final_project.ipynb`: all stages (data, baselines, MLP, SOM, CPN, optimizers, CNN, evaluation, XAI)
- `models.py`: PyTorch MLP and 1D-CNN
- `inference.py`: scoring script (MLP)
- `models_saved/`: trained weights, preprocessors, config
- `results/`: experiment log (`experiment_log.csv`), tables, figures

Random seed: 42 (Python, NumPy, PyTorch). Splits are grouped by student.
"# Artificial-intelligence-and-neural-networks" 
