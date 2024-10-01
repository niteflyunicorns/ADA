# ADA: **A**nomaly **D**etection in **A**steroids

## Background
There are millions of asteroids in our solar system, and every so often, some of them start to display characteristics - such as a tail or comas, like comets do - that asteroids aren't supposed to get. The goal of ADA is to detect the anomalies in an individual asteroid's behaviour from data alone and then send notifications to the public regarding these detections. Currently, ADA runs on data from the Zwicky Transient Facility in Southern California, but we are currently in the process of gearing up to use data from the LSST at the Vera C. Rubin Observatory in Chile, which is expecting first light in January 2025. ADA is an anomaly detection program designed for the **S**olar System **N**otification **A**lert **P**rocessing **S**ystem (SNAPS), which is an Rubin-approved alert broker. 

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites
Make sure you have the following installed on your system:
    
1. Python: Version 3.7 or higher. You can download it form [here](https://www.python.org/downloads/).

2. Anaconda3: A distibution of Python and R for scientific computing and data science.
Download it from [here](https://docs.anaconda.com/distro-or-miniconda/).

3. PyMongo: To interact with MnogoDB using Python.
    - Install using Conda:
        
        `conda install -c anaconda pymongo `

    - Or using Pip:

        ` pip install pymongo `

4. Matplotlib: for data visualization. 
    - Install using Conda:

        `conda install matplotlib `
    
    - Or using Pip:

        ` pip install matplotlip `


2. **Python Version**: Make sure your device is comptiable Python version 3.7 or higher.

### Knowledge Requirments
1. **Python Basics**: Knowledge of Python programming, including with working with libraries, functions, and handling data structures like lists, dictionries, etc. 

2. **MongoDB**: Understanding of NoSQL database, MongoDB's structure (databses, collections, documents), and CRUD operations (Create, Read, Update, Delete) using PyMongo. 

3. **Data Visualization**: Famililarity with Matplotib, including creating basic plots like line charts, bar charts, scatter plots, and customizing graphs. 

### Installation
1. Clone the Repository
    
    Clone this repository to your local machine: 

    `git clone https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository`

    Navigate to the project folder:

    `reqFiles`

2. Download the Data

This project uses a specific dataset stored in MongoDB. Ensure you have access to the MongoDB instance with the necessary credentials (username and password). Make sure to update the connection string in the code with your own credentials:

`mongodb://<username>:<password>@your-mongo-host:your-mongo-port/your-database`


### Running the Project
1. Provide Inputs

    Before running the script, ensure you provided the necessary inputs required by the shell script. Modify the shell script as necessay to match your enviroment. (e.g., database connection details, input files, etc.)

2. Run the Shell Script

    After setting up everything, run the shell script to execute the project: 
    
    `./run_script.sh`

    If the script is not executable, you may need to give it executable permissions:

    ```
     chmod +x run_script.sh
     ./run_script.sh
    ```
## Contributing


## Learn More