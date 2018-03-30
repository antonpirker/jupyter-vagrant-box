# jupyter-vagrant-box

This is a simple Vagrant virtual machine. It contains a setup for running Jupyter notebook with Python 3.

### Prerequisites

You need the following installed on your computer:
- [Virtualbox](https://www.virtualbox.org/)
- [Vagrant](https://www.vagrantup.com/)

### Usage

- Copy `Vagrantfile` and the `scripts` folder to the directory where your data science projects lives.
- Run the shell command `vagrant up` in the folder you copied the files to.
- Wait until the virtual machine is setup and ready.
- Point your browser to [http://localhost:8000](http://localhost:8000)
- **Optional:** If you need to install additional Python packages (or do something similar) you can log into the virtual machine by calling `vagrant ssh`.

That's it. I hope this is useful for some people. Have fun!


### Thank's

Thank's to [Florian Demmer](https://github.com/fdemmer) for helping with the Vagrant provisioning.
