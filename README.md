Install the LarvSeg package in developing mode
pip install -e .
Training command:
bash tools/dist_train.sh <path_to_config>
Evaluation command:
bash tools/dist_test.sh <path_to_config> <path_to_checkpoint> <num_gpus> --eval mIoU
