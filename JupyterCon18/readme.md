# JupyterCon18 - the project jupyter conference
# Abstract
In this repo I document my experience at the JupyterCon18 conference. This readme file serves as an outline for a talk on that experience. First I will set the tone for what the conference was like. Then get straight into what materials I present in the repository. This includes how to find videos and slides from the conference. Then I discuss the sessions I attened and will focus on three main pieces:
1. What Jupyter Is - a demonstration of the Amazon SageMaker to host notebooks (part of AWS)
2. How Jupyter impacts research - the open data lab and other efforts like pangeo
3. How Jupyter impacts education - the educational uses of jupyter notebooks


## "I was there for four days and never opened Jupyter, so what does that tell you"
## "I was there for four days and looked at tons of source code on GitHub"

### Materials
* [Keynotes on Youtube](https://www.youtube.com/playlist?list=PL055Epbe6d5b572IRmYAHkUgcq3y6K3Ae)
* [Video of talks - may not be posted yet](https://www.safaribooksonline.com/library/view/jupytercon-new-york/9781492025818/)
* [Slides from most presentations](https://conferences.oreilly.com/jupyter/jup-ny/public/schedule/proceedings)
* [What I attended](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/agenda.md)

### Terminology
* Project Jupyter - https://en.wikipedia.org/wiki/Project_Jupyter
  * non-profit organization
  * "develop open-source software, open-standards, and services for interactive computing across dozens of programming languages."
  * Spun-off from IPython in 2014 by Fernando Pérez,
  * supports many languages: big 3 are Julia, Python, and R
* Jupyter Notebook
  * web-based interactive computational environment
  * this is where you code [example](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/rkernel.png)
* Jupyter Hub
  * multi-user server for Jupyter Notebooks
  * used in [data8](http://data8.org/) class at berkeley (for example)
* JupyterLab
  * next-generation user interface for Project Jupyter
  * The first stable release was announced on February 20, 2018.


### Amazon SageMaker - (live demo)
* [From Amazon](https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html)
  * fully managed machine learning service
  * integrated Jupyter authoring notebook instance
  * Training and hosting are billed by minutes of usage
* Lets you stand up jupyter notebooks on AWS, preloaded with ML tools like TensorFlow, also spark
* Machine Learning capabilities for training and deployment (includes hyperparameter tuning)

### The Open Data Lab and Project Jupyter - (how to use jupyter for research)
* Here at UVA we have established the [Open Data Lab](https://github.com/UVA-DSI/Open-Data-Lab)
* Ryan Abernathy (Columbia) [gave a keynote talk](https://www.youtube.com/watch?v=7kDYfUe0Zhw&index=12&list=PL055Epbe6d5b572IRmYAHkUgcq3y6K3Ae&t=0s) about a lot of the same principles
* He also [gave a great talk](https://cdn.oreillystatic.com/en/assets/1/event/285/Pangeo_%20Big%20data%20climate%20science%20in%20the%20cloud%20Presentation.pdf) about PANGEO a similar effort for environmental science data.
* Therein he outlines the past/present/future of computing in his field and I think it has some relevance to our efforts
  *  [the past](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/past.png)
  *  [the present](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/present.png)
  *  [the future](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/future.png)

### They had a room dedicated to Education - (how to use jupyter for education)
* What's going on at Berkely?
  * http://data8.org/
  * https://data.berkeley.edu/education/courses/data-8
  * 1,300 students using JupyterHub (the class meets where the symphony plays)
  * https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/data8.png
  
* What's going on in high school?
  * [my favorite slide all conference](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/noTIcalc.png)
  * equip classrooms with chromebooks ~$130/unit (computing power is on the jupyterhub side)
  
* Jupyter Hub
  * [schematic diagram](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/hubdiagram.png)
  * [small scale hub](https://github.com/UVA-DSI/conferences/blob/master/JupyterCon18/images/littlesthub.png)
