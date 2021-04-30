# View tensorboard logs for notebooks launched from SageMaker Studio
## Steps

- From SageMaker Studio Launcher Window, launch the System terminal (under Utilities and files) and run the below commands

  ```pip install tensorflow```

  ```tensorboard --logdir ./logs/fit```

- Launch a notebook from launcher and setup TensorboardCallback to `logs/fit` ([sample](tensorboard_sample.ipynb) in this repo uses tensorflow-2.3-cpu-py37)

- Copy the studio url and replace **lab?** with **proxy/6006/**

  - Example

    Studio Url - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**lab?**

    After Replace - `https://xx.studio.region.sagemaker.aws/jupyter/default/`**proxy/6006/**
