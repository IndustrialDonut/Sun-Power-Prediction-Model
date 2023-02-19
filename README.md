# Sun-Power-Prediction-Model

This uses transfer learning in Pytorch on a pretrained Resnet18 model, to do a regression learning on _the power of the sun_ in as specified in the Bender scene. The end model will give us what it thinks the actual value of the sun is set to, vs what we labelled the pictures with that it actually is.

To use, first make sure you have installed Pytorch with Jupyter Notebook, and Blender.

1. Open the Blender file called DataGenerator, and go to the Scripting tab. Set your output path where you desire, then make sure you have the SUN selected, and run the script. This will generate your training and validation data which is too large to host on github.

![image](https://user-images.githubusercontent.com/76419762/219966813-51b6b96d-35e8-4341-8b98-37c25d20371d.png)

2. Open the jupyter notebook, and set your paths to the training and validation directories as you had generated from blender.

3. Run the notebook! It should start printing out epochs with losses, and by the end give a prediction of the power of the sun in each picture from the validation set, like so:

![image](https://user-images.githubusercontent.com/76419762/219967048-15f18fb2-a623-473f-b215-c218c2c7c3c3.png)
