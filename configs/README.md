### The following are the parameters that can be easily configured by the users:

  - setting: Type of learning method
  - dataset
    - name: Name of the dataset
    - datadir: Directory where the dataset exists/ to download
    - feature: dss/classimb
    - type: pre-defined
  - dataloader
    - shuffle: Reshuffle the data during every epoch
    - batch_size: Number of samples per batch
    - pin_memory: To transfer fetched data to CUDA enabled GPUs
  - model
    - architecture: Network architecture used for training
    - type: pre-defined
    - num_classes: Number of target classes in the dataset
  - ckpt
    - is_load: To load previously saved checkpoint
    - is_save: To save checkpoints
    - dir: Directory to save the model checkpoints
    - save_every: Save every N epochs
  - loss
    - type: loss function
    - use_sigmoid: True/False
  - optimizer
    - type: Type of optimizer
    - momentum: Momentum factor
    - lr: Learning rate
    - weight_decay: Weight decay
  - scheduler
    - type: Type of scheduler
    - T_max: Maximum number of iterations
  - dss_strategy
    - type: Subset Selection Algorithm
    - fraction: Percentage of data used for training
    - select_every: Subset selection every N epochs
    - kappa: Kappa value
    - lam: Lambda value
    - valid: For class imbalance training
  - train_args
    - num_epochs: Number of epochs to train the model
    - device: Device used for training - CPU/GPU
    - print_every: Print every N epochs
    - results_dir: Output log directory
    - print_args: Values to be logged to file - val_loss, val_acc, tst_loss, tst_acc, trn_loss, trn_acc, subtrn_loss, subtrn_acc, time
    - return_args: Arguments to be returned
