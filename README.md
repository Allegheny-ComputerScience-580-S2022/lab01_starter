# cs580-S2022-lab01-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this repository contains the starter files.

## Introduction

### Tutorial for software resource

In this work, you will be studying a software resource (for example, open-source tool or library or web-based tool) of your choice which has some benefit to your own work. As you study this new software, you will be taking notes over how to use it so as to save you time in the future when you are using the software for your research.

Your notes will contain the details of where the software can be obtained and how to install it for your work. In addition, your notes will also contain the details concerning how (where and when) to run and use the software resource. For now, we will assume that the research idea that you presented during a recent lightning talk would benefit form the application of this software resource.

### What to do

In this lab, you are to create a _tutorial-styled_ formatted guide written in Markdown (of about 1000 words) to facilitate a user to understand and apply a chosen software resource. For example, such a guide would have a similar _look and feel_ to the following type of online resource for writing Sockets code in Python; https://realpython.com/python-sockets/.

In clear and meaningful language, please include the following in your tutorial;

 - table of contents,
 - code snippets,
 - screenshots,
 - other necessary details that inspire you from the above example tutorial

#### Writing


In the `writing/tutorial.md` document, please respond to the leading questions below concerning the resource. As you write your tutorial, you may decide that additional details ought to be addressed in the tutorial to inform and instruct the user (i.e., data, algorithms, implementation or similar) and in such cases, please proceed to address these avenues of discussion in your tutorial.

Note: To add screenshots to your work, please use the the following code;
```
![graphic](graphic.png)
```

The following html code serves to scale-down your graphic.

```
<img src="graphic.png" alt="drawing" width="200"/>
```

## Learning

If you have not done so already, please read all of the relevant [GitHub Guides](https://guides.github.com/) that explain how to use many of the features that GitHub provides. In particular, please make sure that you have read the following GitHub guides: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/), [Hello World](https://guides.github.com/activities/hello-world/), and [Documenting Your Projects on GitHub](https://guides.github.com/features/wikis/). Each of these guides will help you to understand how to use both [GitHub](http://github.com) and [GitHub Classroom](https://classroom.github.com/).

## Testing your assignment
This assignment uses [Docker](https://www.docker.com) and [GatorGrader tool](https://github.com/GatorEducator/gatorgrader) to check whether your assignment satisfies the minimum submission requirements. First, you need to make sure you have installed the [GatorGrader tool](https://github.com/GatorEducator/gatorgrader) to verify that the minimal content of your reflection document satisfies the Desktop](https://www.docker.com/products/docker-desktop) and have it running. Then, you can use you can use the [GatorGrader requirements specified in the lab assignment sheet. To run the GatorGrader application to start `gradle grade` as a containerized application, using the [DockaGator](https://github.com/GatorEducator/dockagator) Docker image available on [DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator). First, to ensure that the following command will work correctly, you must create the cache directory by running the command `mkdir $HOME/.dockagator`. Then, to see if your submission satisfies the minimal requirements, you can run the following command in the terminal:

```
docker run --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator
```

This command will use `"$(pwd)"` (i.e., the current directory) as the project directory and `"$HOME/.dockagator"` as the cached GatorGrader directory. Please note that both of these directories must exist, although only the project directory must contain something. Generally, the project directory should contain the source code and technical writing of this assignment, as provided to a student through GitHub. Additionally, the cache directory should not contain anything other than directories and programs created by DockaGator, thus ensuring that they are not otherwise overwritten during the completion of the assignment.  If the above `docker run` command does not work correctly on the Windows operating system, you may need to instead run the following command to work around limitations in the terminal window:


```
docker run --rm --name dockagator -v "%cd%:/project" -v "%HomeDrive%%HomePath%/.dockagator:/root/.local/share" gatoreducator/dockagator
```

Please note; in the settings of Docker, your virtual drive must be shared for this command to work in Windows.
