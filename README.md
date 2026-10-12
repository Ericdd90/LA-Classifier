## Installation
Install LA-Classifier in development mode:

```bash
pip install -e .
Training
Run distributed training. Replace <path_to_config> with your config file path.
bash tools/dist_train.sh <path_to_config>
Evaluation
Run distributed evaluation and calculate mIoU.
<path_to_config>: path to model configuration file
<path_to_checkpoint>: path to model checkpoint
<num_gpus>: number of GPUs used for evaluation
bash tools/dist_test.sh <path_to_config> <path_to_checkpoint> <num_gpus> --eval mIoU

