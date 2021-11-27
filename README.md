<h1 align="center">Movie Recommendation System 🎬🎥🎞️</h1>

## Purpose of Repository:
Repository will contain files for the DSCI final project, part of MS DS course work at RIT - Fall 2021. Please pull or fork the code from this repository and modify as per your requirement.  


## About Data source:
Data files contain 1,000,209 anonymous ratings of approximately 3,900 movies 
made by 6,040 MovieLens users who joined MovieLens in 2000. There are three dataset files included inside the dat_files in this repository.

Filename => Column names

1. users.dat => user_id, gender, age, occupation, zipcode

- UserIDs range between 1 and 6040 
- MovieIDs range between 1 and 3952
- Ratings are made on a 5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)
- Each user has at least 20 ratings

2. movies.dat => movie_id, title, genres

All demographic information is provided voluntarily by the users and is
not checked for accuracy.  Only users who have provided some demographic
information are included in this data set.

- Gender is denoted by a "M" for male and "F" for female
- Age is chosen from the following ranges:

	*  1:  "Under 18"
	* 18:  "18-24"
	* 25:  "25-34"
	* 35:  "35-44"
	* 45:  "45-49"
	* 50:  "50-55"
	* 56:  "56+"

- Occupation is chosen from the following choices:

	*  0:  "other" or not specified
	*  1:  "academic/educator"
	*  2:  "artist"
	*  3:  "clerical/admin"
	*  4:  "college/grad student"
	*  5:  "customer service"
	*  6:  "doctor/health care"
	*  7:  "executive/managerial"
	*  8:  "farmer"
	*  9:  "homemaker"
	* 10:  "K-12 student"
	* 11:  "lawyer"
	* 12:  "programmer"
	* 13:  "retired"
	* 14:  "sales/marketing"
	* 15:  "scientist"
	* 16:  "self-employed"
	* 17:  "technician/engineer"
	* 18:  "tradesman/craftsman"
	* 19:  "unemployed"
	* 20:  "writer"

3. ratings.dat => user_id, movie_id, rating, timestamp

- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres:

	* Action
	* Adventure
	* Animation
	* Children's
	* Comedy
	* Crime
	* Documentary
	* Drama
	* Fantasy
	* Film-Noir
	* Horror
	* Musical
	* Mystery
	* Romance
	* Sci-Fi
	* Thriller
	* War
	* Western

- Some MovieIDs do not correspond to a movie due to accidental duplicate
entries and/or test entries
- Movies are mostly entered by hand, so errors and inconsistencies may exist


### Prerequisites

This is an prerequisites list on things you need to use the software and how to install them.
* [git](https://git-scm.com/download/win)
* [python 3.x.x](https://www.python.org/downloads/)
* [Juptyer Notebook](https://jupyter.org/install) or [Google Colab](https://colab.research.google.com/)
* [Microsoft Visual C++ 14.0 or greater](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

<!-- GETTING STARTED -->
## Getting Started

Install all the prerequisites and follow the installation and how to use guide to use this software.

### Installation and how to use

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Open Command prompt
   by pressing windows + R key together -> type "cmd" -> click ok button
2. Navigate to the respective folder where you want this repo and Clone this repo using the below commands.
   ```sh
   git clone https://github.com/Praveen271195/Movie-Recommedation-System-DRAFT
   ```
3. Install following python packages
   ``` pip3 install wordcloud
   ``` 
4. Open your Juptyer Notebook from the start menu and on File tab navigate to your respective repo folder -> select " Movie Recommendation system - DSCI Final Project.ipynb " file.
5. In Menu -> select Cell -> Run all 

## Content


## Contact US:

Praveen Chandrasekar - pc2846@rit.edu
Ashini Anantharaman - aa9162@rit.edu
Niranjana Sathish Avilery - na6322@rit.edu 
Amit Dilip Kini - ak3328@rit.edu
Vigneshwaran Ravichandran - vr9965@rit.edu

## CITATION:
To acknowledge use of the dataset in publications, please cite the following
paper:

F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History
and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4,
Article 19 (December 2015), 19 pages. DOI=http://dx.doi.org/10.1145/2827872

## Usage License:
Neither the University of Minnesota nor any of the researchers
involved can guarantee the correctness of the data, its suitability
for any particular purpose, or the validity of results based on the
use of the data set.  The data set may be used for any research
purposes under the following conditions:

     * The user may not state or imply any endorsement from the
       University of Minnesota or the GroupLens Research Group.

     * The user must acknowledge the use of the data set in
       publications resulting from the use of the data set
       (see below for citation information).

     * The user may not redistribute the data without separate
       permission.

     * The user may not use this information for any commercial or
       revenue-bearing purposes without first obtaining permission
       from a faculty member of the GroupLens Research Project at the
       University of Minnesota.

If you have any further questions or comments, please contact GroupLens
<grouplens-info@cs.umn.edu>.


## Credits:
Further information on the GroupLens Research project, including research 
publications, can be found at the following web site:
        
        http://www.grouplens.org/

GroupLens Research currently operates a movie recommender based on 
collaborative filtering:

        http://www.movielens.org/


<p align="right">(<a href="#top">back to top</a>)</p>
