# SAC-GIRL





# Dependencies
## Install with pip
* Python>=3.6
* PyTorch>=1.1
* numpy
* tqdm
* cv2
* tensorboard_logger
* imageio (optional, for plots)


# Solving TSP
## Training
```python
CUDA_VISIBLE_DEVICES=0 python run.py --graph_size 20 --seed 1234 --n_epochs 100 --batch_size 512 --epoch_size 5120 --val_size 1000 --eval_batch_size 1000 --val_dataset './datasets/tsp_20_10000.pkl' --no_assert --run_name training
```

## Test only
```python
--eval_only --load_path '{add model to load here}'
```






