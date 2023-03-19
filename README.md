# Notes on running bio related github hosted programs in google colab environment.

## Links

* Keep your session Active:If you are running long running workload, you may want this.

    https://gist.github.com/thomd/f7d8a9c0429c3bb6177237f9a67be775

* How to install and use conda on google colab:

    https://inside-machinelearning.com/en/how-to-install-use-conda-on-google-colab/

* CondaColab example notebook: 

    https://colab.research.google.com/drive/1c_RGCgQeLHVXlF44LyOFjfUW32CmG6BP

## Example Session


  !conda --version

  > /bin/bash: conda: command not found

  !pip install -q condacolab

  import condacolab
  condacolab.install()

  > Once the installation is complete, the kernel should have rebooted itself.

  !which conda
  print(sys.path)

  > To install rdkit library:

  conda install -c conda-forge rdkit
