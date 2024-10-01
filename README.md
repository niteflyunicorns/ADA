# ADA: Anomaly Detection in Asteroids

## Background
There are millions of asteroids in our solar system, and every so often, some of them start to display characteristics - such as a tail or comas, like comets do - that asteroids aren't supposed to get. The goal of ADA is to detect the anomalies in an individual asteroid's behaviour from data alone and then send notifications to the public regarding these detections. Currently, ADA runs on data from the Zwicky Transient Facility in Southern California, but we are currently in the process of gearing up to use data from the LSST at the Vera C. Rubin Observatory in Chile, which is expecting first light in January 2025. ADA is an anomaly detection program designed for the **S**olar System **N**otification **A**lert **P**rocessing **S**ystem (SNAPS), which is an Rubin-approved alert broker. 

## Getting Started
Follow the steps below to set up the environment and run the project.

### Prerequisites
Make sure you have the following installed on your system:
    
1. **Python**: Version 3.7 or higher. You can download it from [here](https://www.python.org/downloads/).

2. **Anaconda3**: A distibution of Python and R for scientific computing and data science.
Download it from [here](https://docs.anaconda.com/distro-or-miniconda/).

3. **PyMongo**: To interact with MongoDB using Python.
    - Install using Conda:
        
        `conda install -c anaconda pymongo`

    - Or using Pip:

        `pip install pymongo`

4. **Matplotlib**: for data visualization. 
    - Install using Conda:

        `conda install matplotlib`
    
    - Or using Pip:

        `pip install matplotlib`


2. **Python Version**: Make sure your device is compatible with Python version 3.7 or higher.

### Installation
1. **Clone the Repository**
    
    Clone this repository to your local machine: 

    `git clone https://github.com/niteflyunicorns/ADA.git`

    Navigate to the project folder:

    `ADA`

2. **Download the Data**

This project uses a specific dataset stored in MongoDB. Ensure you have access to the MongoDB instance with the necessary credentials (username and password). To ensure security in the MongoDB, this project uses a config file, which github then ignores. When you clone the project, make your own `config.ini` file with the following structure, and it will populate the MongoDB connection string with your credentials:

```
[Database]
dbUser = **<username>**
dbHost = **<your-mongo-host>**
dbPort = **<your-mongo-port>**
dbPass = **<password>**
```

### Running the Project
1. **Provide Inputs**

    Before running the script, ensure you provided the necessary inputs required by the shell script. Modify the shell script as necessay to match your enviroment. (e.g., database connection details, input files, etc.)

2. **Run the Shell Script**
    Originally, this project runs on a computing system that utilizes SLURM job scheduling. If you do not have SLURM job scheduling, you can ignore the `#SBATCH ... ` commands at the beginning of the shell script - as they will not affect it.

    After setting up everything, run the shell script to execute the project: 
    
    `./asteroid.sh`

    If the script is not executable, you may need to give it executable permissions:

    ```
     chmod +x asteroid.sh
     ./asteroid.sh
    ```

### Knowledge Requirements
1. **Python Basics**: Knowledge of Python programming, including with working with libraries, functions, and handling data structures like lists, dictionries, etc. 

2. **MongoDB**: Understanding of NoSQL database, MongoDB's structure (databses, collections, documents), and CRUD operations (Create, Read, Update, Delete) using PyMongo. 

3. **Data Visualization**: Famililarity with Matplotib, including creating basic plots like line charts, bar charts, scatter plots, and customizing graphs. 

## Contributing


## Learn More

## License
This project is licensed under XXXX - see the [LICENSE.md](/LICENSE.md) file for details.

## Contact
For more details about how to get involved or set up with the project, feel free to each out to us. We are here to provide support and answer any questions you may have. Below are the best ways to contact our team: 
    - **Email**: Send your inquries to [Savannah](chappus.savannah@gmail.com)
	- **GitHub**: Use the issue tracker and comment spaces to communicate, especially if it's directly related to the project. Remember, others benefit from seeing your questions, comments, and process too!

We look forward to hearing from you and ensuring your experience with our project is successful and enjoyable!