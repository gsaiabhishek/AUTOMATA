# AUTOMATA
AUTOMATA is a Gradient Based Data Subset Selection approach for Compute-Efficient Hyper-parameter Tuning. This repository incorporates various existing subset selection strategies for efficient hyper-parameter tuning.

This repository uses the code from [CORDS](https://github.com/decile-team/cords) and [RayTune](https://docs.ray.io/en/latest/tune/api_docs/overview.html) libraries.

### How to run?
* change the hyper-parametertuning (check configs/SL/config_hp_\*.py) and model config files in AUTOMATA/configs/SL/ to your desired configurations
* Run text_run_sl.py for text datasets (or vision_run_sl.py for vision datasets) with appropriate arguments.   
One example with some of the arguments passed is `python3 text_run_sl.py --config_file configs/SL/config_<dataset>.py --config_hp configs/SL/config_hp_hb.py --fraction 0.1 > output.log 2> error.log`
