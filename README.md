# RLProject
This Github repository was created to document the progress with my reinforcement learning solution for the Duckietown competition.
## Schedule
- [x] Creating summary about Duckietown
- [x] Setting up the environment for Duckietown
- [x] Getting started with RL
- [ ] Trying out basic RL algorithms 
- [ ] Trying out the SAC algorithm for the autonomous driving task
- [ ] Implementing SAC in Duckietown
## How to set up everything for Duckietown
Here is a summary on how to set up everything for duckietown. This summary is based on the [duckietown documentation](https://docs.duckietown.org/DT19/AIDO/out/manual.html). They also have an [interactive tutorials](https://www.duckietown.org/research/ai-driving-olympics/get-started) on their website, where they go through these steps.

### 1.Step Creating accounts
1. **Docker Hub account**\
This account is necessary to submit container images. Take note of your USERNAME.
Create an account [here](https://hub.docker.com/).

2. **Duckietown account**\
This account is necessary to interact with the challenges server.
Create an account [here](https://www.duckietown.org/research/ai-driving-olympics/ai-do-register).

### 2.Step Software requirements
1. **Supported platforms**
    1. *Ubuntu 16*\
Ubuntu 16 is the best supported environment.
    2. *Ubuntu 18*\
Ubuntu 18 is the second best supported environment.
The reason it’s not the first is that sometimes there is some confusion regarding Python 2 vs Python 3.
    3. *Mac OS X*\
OS X is well supported; however there are no instructions for certain steps. There is so much divergence in how OS X environments are configured.

> **Note: If you are a Windows 10 user and have never installed Linux before, it might be a bit challenging task. For me installing Linux next to Windows 10 the steps on this [link](https://askubuntu.com/questions/726972/dual-boot-windows-10-and-linux-ubuntu-on-separate-hard-drives
) did the trick. This was one of the most clearest explanation on this topic, that i could find.**


2. **Docker**\
To install Docker on Ubuntu follow these [instuctions](https://docs.docker.com/install/linux/docker-ce/ubuntu/). The installation process should look like [this](https://www.youtube.com/watch?v=i3BxQlNEhuk). (You can install Docker for Mac OS X from the same website.)

3. **Git**\
You probably already have Git. But to check whether or not you have git installed, simply open a terminal window and type "git --version". If you don't have it installed then follow these [instructions](https://www.liquidweb.com/kb/install-git-ubuntu-16-04-lts/) to install it for Ubuntu.

4. **Duckietown Shell**\
Install the Duckietown Shell by following the Installation instructions in the [README](https://github.com/duckietown/duckietown-shell).\
Make sure it’s installed using:

<pre>
$ dts version
</pre>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Authentication token*\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Set the Duckietown authentication token using this command:
<pre>
$ dts tok set
</pre>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This checks that you have a good authentication token:
<pre>
$ dts challenges info
</pre>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*Docker Hub information*\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Set your Docker Hub username using:
<pre>
$ dts challenges config --docker-username &lt;USERNAME&gt;
</pre>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Login to Docker Hub:
<pre>
$ docker login
</pre>

### 3. Step How to check whether the installation was successful?
I would suggest you to create your first submission to make sure everything is set up properly. For this duckietown has a dummy submission that is outside the competitions. Follow the [instractions](https://docs.duckietown.org/DT19/AIDO/out/cm_first.html) to submit.
