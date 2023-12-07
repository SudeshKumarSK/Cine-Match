# Cine-Match: Movie Recommendation System
CineMatch: Final Project of EE 541(Introduction to Deep Learning for Engineers)

## Description

Cine-Match is an advanced movie recommendation system that utilizes the MovieLens Dataset to provide tailored content-based filtering recommendations. Employing the latest in natural language processing with Transformer BERT Embeddings, and sophisticated similarity measures such as Cosine Similarity, the system is designed to match users with movies that resonate with their preferences.

The system's intelligent content-based algorithm is underpinned by a hybrid model that synthesizes both explicit feedback, like user ratings, and implicit behavioral data, such as viewing history. This approach ensures a nuanced recommendation list that is as informed by user behavior as it is by their direct input.


## Contributors:
1. [Ori Shirin](oshirin@usc.edu)
    USC ID: 4014987308
2. [Sudesh Kumar Santhosh Kumar](santhosh@usc.edu)
    USC ID: 4166249920 

## Important Links:
[MovieLens Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)
[Github Repository](https://github.com/SudeshKumarSK/Cine-Match)

## Installation

Clone the repository to your local machine and navigate to the project's root directory. To install the required dependencies, execute:

```bash
pip install -r requirements.txt
```

## Usage
Run the above command to setup your dependencies and we are using Miniconda Environment for this project. The Jupyter Notebooks were created and used in VS Code using the Miniconda kernels.

Checkout [Miniconda YouTube Tutorial](https://www.youtube.com/watch?v=U3VAqCTujpg)

[Miniconda Installation](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)

Within the `Notebooks` directory, you will find Jupyter notebooks that are central to the project:

1. `Exploratory_Data_Analysis.ipynb`: This notebook explores the MovieLens dataset, providing valuable insights that inform the subsequent recommendation models. Intense Data Visualization to visualize the features of the Movies_Metadata Dataset. Data-Cleansing Techniques and Data Combining strategies were applied here.

2. `Content_Based_Filtering.ipynb`: Here lies the implementation of the content-based filtering model, which uses advanced techniques like BERT Embeddings to understand and recommend movies. Cosine Similarity was applied to recommend movies.

3. `Hybrid_Recommender.ipynb`: A sophisticated system that merges collaborative filtering with content-based methods to predict user ratings and recommend movies using BERT Embeddings and Deep Neural Networks.

Run the notebooks sequentially to replicate the analysis and model training processes. Refer to the Project Structure below to understand where you the Datasets need to be downloaded and placed.


## Project Structure

The project is organized into several key directories:

- `Input/`: Houses the datasets and intermediary files used for the analysis and model training. Key subdirectories include:
  - `CleansedData`: Contains cleaned and preprocessed versions of the datasets.
  - `CosineMatrix`: Stores the precomputed cosine similarity matrices.
  (Computation of Cosine similarity matrices are computationally heavy, so they were generated on Google Colab and placed here).
  - `Data`: The original MovieLens dataset files. (Place the downloaded Datasets here)
  - `Embeddings`: Serialized files of BERT embeddings for use in the recommendation models. (Since Generating BERT Embeddings needs GPU, We used Google Colab's Tesla T4 to generate BERT Embeddings, downloaded them, and stored in the Embeddings directory.)

- `Models/`: Expected to store the trained machine learning model files. As these files are large, they are not included in the repository. A list of models with their approximate sizes is provided for reference.

- `Notebooks/`: Contains the Jupyter notebooks detailing the project's data analysis, model training, and recommendation system implementation.

- `Dataset_Description.pdf`: A document providing a detailed description of the datasets used, including metadata and user feedback.

- `requirements.txt`: Lists all the necessary dependencies required to run the project.

## License

Cine-Match is licensed under the MIT License. See the `LICENSE` file for more information.

## Contact

If you have any questions or would like to discuss the project further, please contact us at:

1. Ori Shirin: oshirin@usc.edu
2. Sudesh Kumar: santhosh@usc.edu
