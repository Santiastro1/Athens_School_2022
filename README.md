# Athens_School_2022

[The 4th Summer School of Hel.A.S. 2022](https://helas.gr/school/2022/)

This repository is meant to help the 4th Summer School of Hel.A.S. 2022 (Athens_School_2022) participants to set up a work environment for the hands-on sessions of the workshop, as well as donwload some example datasets to be used during these sessions. 

It is assumed that there exists a **working [anaconda3](https://www.anaconda.com/distribution/) installation** on the target machine. 

## Installation

Clone the repository (from your $HOME directory, i.e., cd ~):

```console
$ git clone https://github.com/Santiastro1/Athens_School_2022.git
```

Change directory into the cloned repository:

```console
$ cd Athens_School_2022
```
Create a new environment:

```console
$ conda env create -f Athens2022_env.yml
```
Activate the new environment:

```console
$ conda activate Athens2022
```
Verify that the new environment was correctly installed:

```console
$ conda env list
```
The name of the new environment, ```Athens2022```, should show up in the list. 

## Testing the conda environment

Before starting with the ```Athens2022``` we highly recommend you to test the conda environment you have just created. 
First, try to open a ```jupyter notebook``` in your brownser.

```console
$ jupyter notebook
```

Now, in order to test some of the python libraries, you will need to download extra files:

### 1- Used by ```yt```: Data files from N-body simulations obtained using a large variety of numerical codes: https://yt-project.org/data/.

Here we will usedata from ART and RAMSES numerical codes so we recommend you to download the following files and move them to the ```Athens_School_2022``` folder:

http://yt-project.org/data/sizmbhloz-clref04SNth-rs9_a0.9011.tar.gz

```console
$ mv ~/Downloads/sizmbhloz-clref04SNth-rs9_a0.9011.tar ~/Athens_School_2022/
```

```console
$ cd ~/Athens_School_2022/
```

```console
$ tar -zxvf sizmbhloz-clref04SNth-rs9_a0.9011.tar

```
```console
$ rm sizmbhloz-clref04SNth-rs9_a0.9011.tar
```

http://yt-project.org/data/output_00080.tar.gz

```console
$ mv ~/Downloads/output_00080.tar.gz ~/Athens_School_2022/
```

```console
$ cd ~/Athens_School_2022/
```

```console
$ tar -zxvf output_00080.tar
```

```console
$ rm output_00080.tar
```

### 2- Used by pynbody:

Download and extract the following files to your Athens_School_2022 folder

http://star.ucl.ac.uk/~app/testdata.tar.gz

```console
$ mv ~/Downloads/testdata.tar ~/Athens_School_2022/
```

```console
$ cd ~/Athens_School_2022/
```

```console
$ tar -zxvf testdata.tar
```

```console
$ rm testdata.tar
```

Now open the ```Athens2022_envtest.ipynb``` in the web brownser and run each one of the cells in order to test the yt, pynbody and ```Python3.7``` libraries installation.

If you succeed on running all cells in this notebook, you are now ready to work on the ```Athens2022``` school hands-on sessions.

If you have had problems on running any of the cells, please get in contact with sroca01 at ucm dot es, in order to have this problems solved before the school starts.

## Updating installation

Should you need to update an already existing ```Athens2022``` environment with a newer ```Athens2022_env.yml``` version:

```console
$ conda env update --name Athens2022 -f Athens2022_env..yml --prune
```

## Contact

In case of trouble with the installation please contact Santi Roca-Fàbrega (sroca01 at ucm dot es) or open an issue [here](https://github.com/Santiastro1/Athens_School_2022/issues).
