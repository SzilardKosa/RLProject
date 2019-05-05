# Learning to Drive Smoothly in Minutes

Learning to drive smoothly in minutes, using a reinforcement learning algorithm -- Soft Actor-Critic (SAC) -- and a Variational AutoEncoder (VAE) in the Donkey Car simulator.


Blog post on Medium: [link](https://medium.com/@araffin/learning-to-drive-smoothly-in-minutes-450a7cdb35f4)

Video: [https://www.youtube.com/watch?v=iiuKh0yDyKE](https://www.youtube.com/watch?v=iiuKh0yDyKE)

Original github repository: [https://github.com/araffin/learning-to-drive-in-5-minutes](https://github.com/araffin/learning-to-drive-in-5-minutes)

## Some tips for running the repository above

### First tip: Installing the simulator
You can find most of the steps to run the project on the original github repository under Quick Start. The only thing that wasn't clear is how to install and use the simulator. It is the 0. point in the Quick Start. It says you can download it or build it from source. I used the first option. It is important, that you have to have [Unity](https://unity3d.com/get-unity/download) installed. Linux Unity install [here](https://forum.unity3d.com/threads/unity-on-linux-release-notes-and-known-issues.350256/). Check last post in this thread. I used Ubuntu 16.04., so I used the later link.

### Second tip: Installing Unity on Linux
I found [this link](https://askubuntu.com/questions/1035566/how-do-i-install-the-latest-unity3d-beta-unitysetup-2018-1-0f2-on-ubunu-18-04-l) very helpful, for installing Unity on Linux. After I installed Unity, I was able to run the downloaded simulator.

### Third tip: Running the scripts
At the third step of the Quick Start, it forgets to mention, that you have to start the simulator before starting the training.
