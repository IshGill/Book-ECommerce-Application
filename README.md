# Book E-Commerce Web Application


# Description
## Home Page

-	We focused on designing the webpage with an elegant aesthetic styling, which was simple to digest for the user, hence, void of clutter and excess content. We also wanted to be able to portray to the user the various functionalities our web page has just from the home screen. For example, the ability to search for books by title and the tabs on the navigation bar which show authentication, reading list and browsing by feature functionalities of our webpage.

## Browsing books by category

-	We have implemented three separate browsing categories for the user where the user 
is able to sort books by their preference of date, author, and publisher. In the example above we have a user which has sorted the books by date.

## Book Searching

-	As we stated previously in the home page description, this website has the added functionality where the user is able to query books which exist in the database via title. 
-	This feature is able to pick up all books which contain the specified search query within their title.


## User Authentication

-	We have implemented full user authentication features into this website, where a user is able to register, login and interact with the special features of the website which we will discuss shortly.
-	We have implemented SOLID principles, in particular the Single Responsibility Principle when implementing our authentication features for this website. 
-	We have also used WTForms and appropriate HTML forms when implementing the authentication related features. 

## Reviewing Books

-	An authenticated user is able to post reviews on books which they have read via the book page and the Write a Review button. 
-	The reviews are based on a 0-to-5-star system, and we have implemented WTForms into our reviewing system, as to avoid cuss words and invalid user input as reviews. 
-	If a user is not authenticated, the webpage will redirect the user to the login page where they must login in order to place their review.
-	We have applied a multitude on unit tests in order to test the functionality of our review system also.

## Reading List

-	This is a brilliant feature where a logged in user is able to browse our selection of books via the home page, then by clicking on a particular book which they are interested in on the home page, the user is redirected to the books page, where they can find a button which allows them to add this particular book to their personal reading list. 
-	There is no limit on the number of books a user can add, and whenever the user is finished with the book, they are able to click on the book in question to go to that books page and remove the particular book from their reading list.
-	If a user is unauthenticated and tries to add a book to their reading list, they will be redirected to the login page. This functionality is present from both the add to reading list button and Reading list tab on the navigation bar.
-	A List ADT was used to implement this feature. 

## User Profile

-	This feature depicts the profile of an authenticated user, where the user is able to keep track of all of the reviews, they have made for books which they have read. 
-	We believe this is an important feature a user would enjoy as if for example, they wanted to re-read a book which they previously appreciated.

## Rating, price, and stock system

-	As you may have noticed from the home page, each book icon has a very aesthetic design which features tags depicting the price and current stock of each individual book. 
-	We also have implemented a rating system, which is based on 5 stars. Therefore, every user is able to view the number of ratings and average rating of a book which they may be interested in reading. 
-	These pricing, stock and rating details are once again reiterated in the product details section of the books page, alongside additional details such as formats available and page, publication, and publisher data. 
-	We would also mention another button which has been added which provides a link to the book on goodreads a popular ecommerce book page, which we believe is a valuable addition if the user is interested in purchasing the particular book.
This concludes the highlights of the various features of our web application. We would also mention we have thoroughly tested all of the various components of our web application with the pytest software testing framework. This is done in order to ensure the user has a seamless error free experience and is able to enjoy the many special features available on our website.
Thank you for viewing our project
Team A

# Python version

Please use Python version 3.6 or newer versions for development. Some of the depending libraries of our web application do not support Python versions below 3.6!

# Installation

**Installation via requirements.txt**

```shell
$ py -3 -m venv venv
$ venv\Scripts\activate
$ pip install -r requirements.txt
```

When using PyCharm for requirements installation, set the virtual environment using 'File'->'Settings' and select your project from the left menu. Select 'Project Interpreter', click on the gearwheel button and select 'Add'. Click the 'Existing environment' radio button to select the virtual environment. 

# Execution of the web application

**Running the Flask application**

From the project directory, and within the activated virtual environment (see *venv\Scripts\activate* above):

````shell
$ flask run
```` 

# Data sources 

The data in the excerpt files were downloaded from (Comic & Graphic):
https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/home

On this webpage, you can find more books and authors in the same file format as in our excerpt, for example for different book genres. 
These might be useful to extend your web application with more functionality.

We would like to acknowledge the authors of these papers for collecting the datasets by extracting them from Goodreads:

*Mengting Wan, Julian McAuley, "Item Recommendation on Monotonic Behavior Chains", in RecSys'18.*

*Mengting Wan, Rishabh Misra, Ndapa Nakashole, Julian McAuley, "Fine-Grained Spoiler Detection from Large-Scale Review Corpora", in ACL'19.*
