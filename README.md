<h1 align="center">Movie Recommendation System 🎬🎥🎞️</h1>

## Objective:
Repository will contain files for the DSCI-633: Foundations of Data Science and Analytics final project, part of MS DS course work at RIT - Fall 2021. Our Recommendation system's main goal is to filter and predict only those movies that a user would like based on the individual data provided by the user. Different implementation applied to this project is Content Based Model and Collaborative Filtering Model. Our learning objective were initially we worked on the Content Based model to predict the movies for recommendation, but the downside of the model is that it predicted the top 10 movies based on the genre provided by the user and not by the user preference. Based on the above reasons which provided same movies set for all user since it was based on genre, we moved onto the next model which is the Collaborative Filtering which create a model based on the user's past behavior (i.e., movies seen or searched in the past) as well as identical decisions made by other users. This model is then used to predict which movie (or ratings) users might be interested in. Collaborative filtering is more efficient on this project than the Content Based model. To working on this project, take a pull or fork the code from this repository and modify as per your requirement.


## About Data source:
 As per the data source, all the Data files contain 1,000,209 anonymous ratings of approximately 3,900 movies 
 made by 6,040 users who joined the service in 2000. There are three data set files added inside the dat_files folder for this project. The file format of the data set file is .dat format. These .dat format files are further processed and converted into CSV files and saved in the root directory then those files are further used on the project. The reason for choosing this dataset is that it has a reasonable amount of rows on each file. It also had both categorical and continuous data. It also helps us achieve our target goal of predicting movies based on user preference.

### User.dat file description

user_id :: gender :: age :: occupation :: zipcode
				
Data source provided the information that all demographic information is provided voluntarily by the users and is
not checked for accuracy.  Only users who have provided some demographic
information are included in this data set.

- UserIDs range between 1 and 604 and also serves as the foreign key for User.dat and Ratings.dat file
- Gender is represented by a "M" for male and "F" for female
- Age is chosen from the following ranges "Under 18" to "56+" years of age:
- There are 21 different Occupation collected by the data source. 

### Movies.dat file description

movie_id :: title :: genres 

- MovieIDs range between 1 and 3952 and also serves as the foreign key for Movies.dat and Ratings.dat file 
- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated | in the same column:
- Some MovieIDs do not correspond to a movie due to accidental duplicate
entries and/or test entries
- Movies are mostly entered by hand, so errors and inconsistencies may exist

### Ratings.dat file description

user_id :: movie_id :: rating :: timestamp

- UserIDs range between 1 and 604 and also serves as the foreign key for User.dat and Ratings.dat file 
- MovieIDs range between 1 and 3952 and also serves as the foreign key for Movies.dat and Ratings.dat file 
- Ratings are made on a 5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)
- Each user has at least 20 ratings


## Online Dataset link

[Link](https://grouplens.org/datasets/movielens/1m/) - Link to the data set.

## Prerequisites

To start using this project with Git, you’ll need to install or have access to the following program. <br/>
- [Git](https://git-scm.com/download/) <br/>
- [Python 3.9.9](https://www.python.org/downloads/) <br/>
- [Juptyer Notebook](https://jupyter.org/install) or [Google Colab](https://colab.research.google.com/) <br/>


## Libraries
- <a href="https://pandas.pydata.org/">Pandas</a>
- <a href="https://numpy.org/">Numpy</a>
- <a href="https://seaborn.pydata.org/">Seaborn</a>
- <a href="https://matplotlib.org/stable/tutorials/introductory/pyplot.html">Matplotlib Pyplot</a>
- <a href="http://amueller.github.io/word_cloud/">Wordcloud</a>


## Method used:
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html">Tfidf Vectorizer</a>
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.linear_kernel.html">Linear kernel</a>
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html">Cosine similarity</a>
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html">Train test split</a>
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise_distances.html">Pairwise distances</a>
- <a href="https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html">Mean squared error</a>



## Getting Started

### Installation

#### Git
Git can be installed using a CLI or an executable file. The installation instructions can be found at the following link:[Windows](https://git-scm.com/download/win) or [Mac OSX](https://git-scm.com/download/mac)


#### Python and Jypter Notebook
If you have not installed Python 3.9 already, the easiest method to install both the programs is by installing [anaconda](https://www.anaconda.com/) The following link provides a graphical installer link for both Windows and Mac OS [Link](https://www.anaconda.com/products/individual)

If you have already installed Python 3.9 and are an advanced user, you can install Jypter Notebook on terminal by following the steps below.

	pip3 install jupyter	

### Setting up your local
In Terminal navigate to the respective directory where you want to clone this repository and run the following command <br/>

   ```
   git clone https://github.com/Praveen271195/Movie-Recommedation-System-DRAFT
   ```

If you have forked this repository, use the following code but replace the [username] in the link with your git username.

   ```
   git clone https://github.com/[username]/Movie-Recommedation-System-DRAFT
   ```

### Running the environment

#### Jypter Notebook

If you have installed the Jypter notebook via anaconda, you can run the notebook directly by double clicking on the Jypter notebook icon on the start menu on Windows or Mac, going to the app drawer and selecting the Jypter notebook.

If you have installed Jypter notebook via Python, you can go to Terminal and type the following code:
 
   ```
   jupyter notebook
   ```

Both the processes will open up the Jypter notebook environment in a default web browser. 

In the application window, there will be a file explorer. Navigate to the respective folder where you have cloned the project and select the **" Movie Recommendation system - DSCI Final Project.ipynb "** to load up the notebook. 

#### Google Colab

If you want to run this project on Google Colab, Navigate to the following [link](https://colab.research.google.com/)

In the application window, click on File->Open Notebook from the menu tab or press Ctrl + O. On the open popup model, click on upload file and go to the respective folder where this project is cloned and select the **" Movie Recommendation system - DSCI Final Project.ipynb "** so that it can be uploaded to Google Colab.

### Running the project
 
5. In Menu -> select Cell -> Run all 


## Project members:

[Amit Dilip Kini](mailto:ak3328@rit.edu) <br/>
[Ashini Anantharaman](mailto:aa9162@rit.edu) <br/>
[Niranjana Sathish Avilery](mailto:na6322@rit.edu) <br/>
[Praveen Chandrasekar](mailto:pc2846@rit.edu) <br/>
[Vigneshwaran Ravichandran](mailto:vr9965@rit.edu) <br/>

## Data Usage License:
Neither the University of Minnesota nor any of the researchers
involved can guarantee the correctness of the data, its suitability
for any particular purpose, or the validity of results based on the
use of the data set.  The data set may be used for any research
purposes under the following conditions:

 - The user may not state or imply any endorsement from the
   University of Minnesota or the GroupLens Research Group.

 - The user must acknowledge the use of the data set in
   publications resulting from the use of the data set
   (see below for citation information).

 - The user may not redistribute the data without separate
   permission.

 - The user may not use this information for any commercial or
   revenue-bearing purposes without first obtaining permission
   from a faculty member of the GroupLens Research Project at the
   University of Minnesota.

If you have any further questions or comments, please contact GroupLens
<grouplens-info@cs.umn.edu>.

## Citation:
To acknowledge use of the dataset in publications, please cite the following
paper:

F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History
and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4,
Article 19 (December 2015), 19 pages. DOI=http://dx.doi.org/10.1145/2827872


<p align="right">(<a href="#top">back to top</a>)</p>
