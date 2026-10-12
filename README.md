
## Installation

Install LA-Classifier in development mode:

```bash
pip install -e .
```

## Training

Run distributed training. Replace `<path_to_config>` with your config file path.

```bash
bash tools/dist_train.sh <path_to_config>
```

## Evaluation

Run distributed evaluation and calculate mIoU.

- `<path_to_config>`: Path to model configuration file.
- `<path_to_checkpoint>`: Path to model checkpoint.
- `<num_gpus>`: Number of GPUs used for evaluation.

```bash
bash tools/dist_test.sh <path_to_config> <path_to_checkpoint> <num_gpus> --eval mIoU
```
