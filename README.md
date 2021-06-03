# Launching TensorBoard from SageMaker Studio

## Steps 
 
- Select a SageMaker Studio Image

![select_image](./images/select_image.png)
  
- Launch & Run a notebook from launcher and that uses TensorboardCallback ([sample](tensorboard_sample.ipynb) in this repo uses tensorflow-2.3-cpu-py37)

![launch_notebook](./images/launch_notebook.png)

- From SageMaker Studio's Jupyter Server, launch the System terminal (under Utilities and files) 

![](./images/launch_system_terminal.png)

- Run the following commands. Get the EFS path for the logs folder. (check the EFS_PATH_LOG_DIR variable in the sample notebook as an example)

  ```pip install tensorboard```

  ```tensorboard --logdir {EFS_PATH_LOG_DIR}```
  
  ![install_tensorboard](./images/install_tensorboard.png)
  
- Copy the studio url and replace **lab?** with **proxy/6006/**

  - Example

    Studio Url - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**lab?**

    After Replace - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**proxy/6006/**

![view_tensorboard](./images/view_tensorboard.png)
