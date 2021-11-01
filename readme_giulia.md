- In pytorch_lightning/loggers/mlflow.py, in `MLFlowLogger` class (__init__() method):
  
  `run_id` is made attribute of the class and is initialized to `None`.

  This was done in order to decide the id of the run.


- In pytorch_lightning/callbacks/progress.py:

  instead of `from tqdm.auto import tqdm as _tqdm`:

  `from tqdm.notebook import tqdm as _tqdm`.

  This was done in order to visualize a compact progress bar during training.