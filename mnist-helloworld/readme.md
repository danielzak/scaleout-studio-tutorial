# Mnist tutorial

This is a hello world example of Scaleout Studio using the mnist datset for handwritten digit recognisation. 


This is a good first example that will go through the basics of creating a new Studio project and then creating a Jupyter notebook in a new Lab environment. 

Needed:
A user account in a Scaleout Studio installation

## Create a new project
Projects are the highest level of separation in Studio. Each project can have many different workflows, models and datasets, but these are not shared directly between projects.

1. Go to https://platform.demo.scaleout.se/ 
2. Click _Projects_ in top bar
3. Enter name **Minst Hello World** and click _Create project_

## Create a new Lab session
Labs is the work area for experimentation and development of machine learning projects. It's based on Lab Sessions which is a provisioned Jupyter Notebook session running in a virtual environment.

In the most simple case, everything to run a machine learning experiment is cointained within one Labs Session, which is what we will do now.

1. Click Labs in the left menu
2. Start a labs session image based on _jupyter/minimal-notebook_latest_ 
3. Select _1 CPU_, _2 RAM_ to start receive an instance with 1 virtual CPU and 2 GB ram from the Kubernestes cluster.
4. Wait for a minute and click the link to the notebook in the list under Lab Session

## Add required modules to the instance
We need to add some additional Python modules to the setup provided in the minimal-notebook. There are several ways to do this, but we'll install using pip in the Jupyter Terminal.

1. Open Jupyter Terminal by clicking the + sign in the top left corner and select _Terminal_ (under other)
2. Install tensorflow in the terminal by entering **pip install tensorflow**. 
3. When the status indication in the bottom left corner says _Idle_ (it can be _Busy_ or _Idle_), install Matplotlib by entering **pip install matplotlib** 
4. Run **pip freeze** to check installed Python libraries. _tensorflow_ and _matplotlib_ should now be in the list.

## Run the notebook 
In this folder there is a full Jupyter notebook with the example. You can upload it to the Lab session and just run it, or open it on your computer and work through the example line by line.
