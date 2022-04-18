# workshop-time-series

## Install Python and Anaconda
The environment setup was done using the Windows operating system.
To do this, students must have the following tools installed:
- [Python](https://www.python.org/downloads/) - Don't forget to check the 'Add to Path' option during the installation.
- [Anaconda](https://www.anaconda.com/)

## Add Python and Anaconta to Windows Environment Variables
The *'pip'* and *'conda'* commands, from Python and Anaconda, respectively, allow us to install the necessary packages for this workshop from the terminal (cmd in Windows). To use these commands, we have to add the Python and Anaconda paths to the Windows environment:

1. Open the Windows System Environment variables
<img src="https://user-images.githubusercontent.com/32846089/163836636-4810e142-b5de-40ab-a724-4294734434b7.png" alt="drawing" width="400"/>
<img src="https://user-images.githubusercontent.com/32846089/163840743-e35cfdd7-cc90-4469-96fa-89f3466f4cb7.png" alt="drawing" width="400"/>
<img src="https://user-images.githubusercontent.com/32846089/163841399-0be15c7f-0a45-483d-9821-76ac75d0b358.png" alt="drawing" width="400"/>

Now you can add a new path to the Windows environment. Following there are the paths being added for Python and Anaconda.

> Note: Bearing in mind that my Windows username is 'joao.miguel', you will have to use your username instead, and verify that the path exists (and that both tools were installed correctly).

2. Add Python to the Path variable

If the 'Add to Path' option was checked during the installation of Python, this step will probably not be necessary.
<img src="https://user-images.githubusercontent.com/32846089/163843784-4713bbd5-6847-492d-9df7-af1574a8c241.png" alt="Python Path" width="400"/>

3. Add Anaconda to the Path variable
<img src="https://user-images.githubusercontent.com/32846089/163835982-c002cf65-16ed-4e17-b6a8-17f286e6269c.png" alt="Anaconda Paths" width="400"/>

It should now be possible to use the *'pip'* and *'conda'* commands in the Command Prompt (also known as cmd) to install the packages that will be used in this workshop. To confirm, try running the following commands:

> pip --version

> conda --version

## Create New Environment using Anaconda

Download the *'workshop-students'* folder, present in this repository, to your computer's desktop. Then open a Command Prompt (cmd) and enter the folder you downloaded using the command *'cd'* followed by its location:

> cd Desktop\workshop-students

<img src="https://user-images.githubusercontent.com/32846089/163880868-beeff278-612e-440f-adaa-877ca084a5ea.png" alt="" width="500"/>

Now let's create and activate a new environment with a specific Python version (3.8) using *'conda'*. This step was done to avoid conflicts between the new Python versions and the Prophet model library. For such, use the following commands to create and activate an environment with name *'time_series'*.

> conda create -n time_series python=3.8

<img src="https://user-images.githubusercontent.com/32846089/163882405-7bedfdb6-edd3-404a-b3a6-ca838e8f2943.png" alt="" width="600"/>

> conda activate time_series

<img src="https://user-images.githubusercontent.com/32846089/163882632-7cbc48db-3619-46c0-ac28-38a0c757bd46.png" alt="" width="600"/>

If everything goes as expected, the environment name will appear in parentheses, indicating that it is activated.

## Install Packages using *'pip'* and *'conda'* commands
