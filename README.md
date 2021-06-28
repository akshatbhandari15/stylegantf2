Preparing Dataset
Use the following command to convert the images to multi-resolution TFRecords:


python dataset_tool.py create_from_images ~/datasets/my-custom-dataset ~/dirOfDataset
python dataset_tool.py display ~/datasets/my-custom-dataset


Make sure you have all the images in one directory and are square-shaped


Use this command to train the model on the dataset:
python run_training.py --num-gpus=1 --data-dir=/home/akshat/datasets --config=config-a --dataset=adni --mirror-augment=true

