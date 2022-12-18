# Netflix-Movies-TV-Shows-Clustering

# Problem Statement-
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.
Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

# Attribute Information-

1) show_id : Unique ID for every Movie / Tv Show

2) type : Identifier - A Movie or TV Show

3) title : Title of the Movie / Tv Show

4) director : Director of the Movie

5) cast : Actors involved in the movie / show

6) country : Country where the movie / show was produced

7) date_added : Date it was added on Netflix

8) release_year : Actual Releaseyear of the movie / show

9) rating : TV Rating of the movie / show

10) duration : Total Duration - in minutes or number of seasons

11) listed_in : Genere

12) description: The Summary description

# Data Cleaning-

**1. Duplicate Values Treatment:**
 • Duplicate values do not contribute anything to the accuracy of results.
 • Our dataset does not contain any duplicate values.

 **2. Null Values Treatment:**
 • Director feature has more than 30% of null values. So, dropping the feature
director.
 • Country feature has 6.51% of null values. Filling null values by mode of the
feature.
 • Cast feature has 9.22% of null values. Filling null values by 'missing’.
 • Rating feature has 0.09% of null values. Filling null values by mode of the feature.
 • Date_added feature has 0.12% of null values. Dropping rows corresponding to null
values.

# Data Pre-processing-

**1. Date Type Change:**
• Features in their appropriate data type provide better understanding and
workability on that data.
• Date_added feature has an object datatype. Converting to DateTime.
• Duration is in a combination of integer values and text. Removing text part so
as to get integer datatype.

**2. New Features:**
• From the feature date_ added; extracted year, month, and day to form new
columns by name of the year, month, and day respectively

# Exploratory Data Analysis - 

**Movies vs TV shows**

• Movies uploaded on Netflix are more than twice the TV Shows uploaded.
• 30% of movies are released on Netflix.
• 70% of movies added on Netflix were released earlier in a different mode.

**On Year Basis**

• TV shows are increasing continuously
• The number of releases significantly increased after 2015 and dropped in
2021 because of Covid 19.

**On Month Basis**

• From October to January, the maximum number of movies and TV
shows were added.
• Possible reason for that is, during this period of time events such 
as Christmas, New Year and several holidays take place.

**On Day Basis**

• Maximum number of movies and TV shows added at the start 
of the month followed by mid of month.

**Worldwide Presence**

• United States tops in the list of the maximum number of movies and TV
shows, followed by India, the UK, and Japan.
• 10th no. of the country is Turkey.

**Ratings**

• Maximum of the movies as well as TV shows are for
matures only.
• we can observe that the most-rated movie on Netflix is TV-MA
and the least-rated movie on Netflix is UR.

**Cast**

• Anupam Kher top of the list of casts having a maximum
number of movies and TV shows.

**Running Time OF movies**

• most of the movies have a duration of between 50 to 150.

**Seasons of TV Shows**

● Almost 68% of TV shows
consist of a single season
only.


