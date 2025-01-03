Programming Workshop Lab Semester Project- Milestone 3 <br>

Purpose:<br>
The purpose of this application is to allow users to process their text article of choice by calculating basic statistics, the word frequency and analyzing the sentiment.<br>

The goal for milestone 1 is being able to process the article, remove stop words and rank words by frequencies. To do this we created 4 classes, an Article class to read the file, store the words to an arraylist and clean the data and process and remove the stop words, count the words and sort them by frequency; a Topic class which calls the functions in the Article class for each article in a topic; and a Library class to processes each topic.<br>

For milestone 2 we compared the articles based on vocabulary and attitude. To calculate the richest vocab, we returned the number of unique words for a given article (Article class). To find the most repeated words we created an arraylist 'frequencies' with frequencies set for each word in 'uniqueWords' and found the maximum value. To do the sentiment analysis we process text files of positive and negative words and store them in arraylists, in the Library class. Then in the Article class we counted the number of positive and negative words appearing in a given article, determining if an article was positive, negative or neutral.<br>
	
For milestone 3 we created a user interface in the Main class for users to choose from a variety of tasks to apply in the application. They have the options to process existing topics and also to create their own folders and add files from their device. We implemented a switch case statement to configure the interface and the users’ inputs. The first three options of the switch case allow the user to choose from existing topics to process. The fourth option allows users to create a new folder by entering their folder name that would be applied to the ‘libraryPath’ by the method and allow for it to show in the applications directory.  The fifth choice allows users to add a file from their device and move it to a folder of choice in the library. The sixth choice allows the user to select any folder to process all the articles it contains. After each task is completed from the options chosen by the user the interface will be prompted again until the user chooses the seventh option to exit.<br>

Credits:<br>
Authors:<br>
Mariella Aletti<br>
Sofia Morgillo<br>
Nazli Yaglidere<br>

Articles Used:<br>
'Nearly a Century Later, We’re Still Reading — and Changing Our Minds About — Gatsby' by Parul Sehgal https://www.nytimes.com/2020/12/30/books/great-gatsby-fitzgerald-copyright.html<br>
'The Great Gatsby by F Scott Fitzgerald - review' by ThePinkElephant https://www.theguardian.com/childrens-books-site/2013/sep/12/review-great-gatsby-f-scott-fitzgerald<br>
'[The Great Gatsby]: A Review' by Jane@GreenishBookshelf https://greenishbookshelf.com/2017/05/31/the-great-gatsby-a-review/<br>

'Book Review: To Kill a Mockingbird (Harper Lee). by Aarti Athavle https://booksandbluess.co.in/2021/04/18/book-review-to-kill-a-mockingbird-harper-lee/<br>
'To Kill a Mockingbird by Harper Lee- review' by David https://www.theguardian.com/books/2013/oct/17/review-to-kill-a-mockingbird-harper-lee<br>
'Book Review: To Kill a Mockingbird' by Ethan M https://ppld.org/book-reviews/kill-mockingbird-1<br>

'The Outsiders by SE Hinton- review' by Hemma https://www.theguardian.com/childrens-books-site/2015/sep/23/the-outsiders-s-e-hinton-review<br>
'Book Review: The Outsiders' by Sophie L. https://ppld.org/book-reviews/outsiders-0<br>
''The Outsiders': 40 Years Later' by Dale Peck https://www.nytimes.com/2007/09/23/books/review/Peck-t.html<br>

Code/Files Used:<br>
Scanner class to read file https://www.geeksforgeeks.org/different-ways-reading-text-file-java/<br>
Split article text to arraylist https://www.w3schools.com/java/ref_string_split.asp<br>
Bubble sort 'CountWords1.java'<br>
Postive and negative words list for determing the sentiment of the articles: <br>
     Minqing Hu and Bing Liu. "Mining and Summarizing Customer Reviews."
 Proceedings of the ACM SIGKDD International Conference on Knowledge
 Discovery and Data Mining (KDD-2004), Aug 22-25, 2004, Seattle,
 Washington, USA <br>

Refactoring Suggestions: 
<br>
The original calculateWordFrequency method in the Article class works to calculate the frequency that a word is present in a cleaned and processed article that has already removed stop words. This method determines the frequencies of each word and prints them in ranked order from most to least frequent for each article. It also determines and prints the word that was repeated most and the amount of times. It avoids complex structures and is straightforward for both developers and the audience to use and understand.

For the calculateWordFrequency method to be improved, it can be refactored to have three separate methods, each with one specific task. Since the method as a whole can calculate the ranking, frequency, and most repeated word, it can also be broken up so each of these tasks have their own method. Refactoring can also increase modularization and strengthen cohesion. This would improve readability and understanding by modularizing and having better organization to help maintain easier. 

Hashmap may be a better option to calculateWordFrequency as it would use key and value pairs where the key is the word and the value is the integer of frequency. Using hashmap can allow quick updates and allow possible manual input when the application needs to be further updated to achieve more goals. It can also be helpful when new features like searching for a word and its frequency are implemented in the application. 
</br>

 UML Diagram:
 <br>
 <img height="500" src="UML_Milestone_3.jpg" />
 </br>

 Screenshot of testing results:
 <br>
 Case 1 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 1.png"/>
 <br>
 Case 2 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 2.png"/>
 <br>
 Case 3 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 3.png"/>
 <br>
 Case 4 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 4.png"/>
 <br>
 Case 5 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 5.png"/>
 <br>
 Case 6 Output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 6.png"/>
 <br>
 Case 7 output:<br>
 <img height="500" src="Programming Lab Milestone 3 Case 7.png"/>
 <br>

