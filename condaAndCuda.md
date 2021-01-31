# Ubuntu 20
Anaconda installation: `https://linuxize.com/post/how-to-install-anaconda-on-ubuntu-20-04/`
<br/>

# Ubuntu 18
Create (and activate) a new environment, named `cv-nd` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.
Anaconda [installation](https://www.digitalocean.com/community/tutorials/how-to-install-anaconda-on-ubuntu-18-04-quickstart) and [installing](https://medium.com/analytics-vidhya/how-i-installed-cuda-10-0-for-pytorch-in-linux-mint-2ce26dd1930f) cuda 10.1 and cudnn for in-built Nvidia GPU. 
Follow the instructions to setup the enviornment in local GPU:
	- __Linux__ : 
	```
	conda create -n cv-nd python=3.6
	source activate cv-nd
	conda install pytorch torchvision cudatoolkit=10.0 -c pytorch
	pip3 install -r requirements.txt
	```
