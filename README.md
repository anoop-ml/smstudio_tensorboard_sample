# Launching TensorBoard from SageMaker Studio

## Steps 

- From SageMaker Studio's Jupyter Server, launch the System terminal (under Utilities and files) 

![](./images/launch_system_terminal.png)

- Run the following commands

  ```pip install tensorboard```

  ```tensorboard --logdir ./logs/fit```
  
  ![install_tensorboard](./images/install_tensorboard.png)
  
- Select a SageMaker Studio Image

![select_image](./images/select_image.png)
  
- Launch a notebook from launcher and setup TensorboardCallback to `logs/fit` ([sample](tensorboard_sample.ipynb) in this repo uses tensorflow-2.3-cpu-py37)

![launch_notebook](./images/launch_notebook.png)
  
- Copy the studio url and replace **lab?** with **proxy/6006/**

  - Example

    Studio Url - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**lab?**

    After Replace - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**proxy/6006/**

![view_tensorboard](./images/view_tensorboard.png)
