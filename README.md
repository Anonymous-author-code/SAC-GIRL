# SAC-GIRL




# Jupyter Notebook
We provide a Jupyter notebook to help you get started and understand our code. Please open the  [notebook here](Solving%20TSP%20with%20Improvement-base%20DRL.ipynb) for more details.

Note: due to the 100MB limit of Github, please download the logs folder for the pre-trained model via [Google Drive](https://drive.google.com/drive/folders/1IaFPXh1IzHz02LqBSRa2wqhPjQ7WksOd?usp=sharing) and put it under './logs/pre_trained/' folder.

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
Note: A pre-trained model can be found at './outputs/tsp_20/tsp_20200714T212735/epoch-99.pt'





