# PCS5024 - Aprendizado Estatístico

## Practice: Classifiers for the Adult Dataset

This project contains a practice assignment for the discipline PCS5024. The goal
of the practice is to train some classifiers on the [UCI Adult Dataset](https://archive.ics.uci.edu/ml/datasets/adult).

## Running the project

### 1. Building the Docker Image

Run the commands below inside the project's root directory.

<pre><code>
cd /path/to/project/root_dir
docker build -t adult .
</code></pre>

### 2. Running Jupyter Notebook on the Docker Container

Run the commands below inside the project's root directory.

<pre><code>
cd /path/to/project/root_dir
docker run --rm -dit --name adult -p 8888:8888 -v $(pwd):/usr/src/code adult kedro jupyter notebook --ip 0.0.0.0
</code></pre>

### 3. Getting the Jupyter Token

Run the comand below to get the address for the Jupyter Notebook Server.

<pre><code>
docker exec adult jupyter notebook list
</code></pre>

### 4. Running the code

The practice code is contained in the notebook located at **/path/to/project/root_dir/notebooks**.


Cheers!

Rodrigo Cunha
