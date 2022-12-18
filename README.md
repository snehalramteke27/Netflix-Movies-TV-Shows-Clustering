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

**2. New Features:
• From the feature date_ added; extracted year, month, and day to form new
columns by name of the year, month, and day respectively
