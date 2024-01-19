# CS412_project
Cs412 term project. Arda Poyraz, Özen Özdemir, Meltem Oras, Berdan Şen, Hakkı Zambak

As we are the group of people Hakkı Zambak, Özen Özdemir, Arda Poyraz, Berdan Şen and Meltem Oras,
we put all our knowledge from the lecture and previous homeworks together. 
We decided to follow the process with cosine similarity, jaccard similartiy, random forrest regression, randomized search and 
hyperparameter to optimize the project. 

First, 
we downloaded the contents by seperating the student's questions and ChatGPT's answers and we listed all the
questions into the question_df. 
After that, we cleaned the question_df words which are "=", "#", "pts)", "line", "file", "use", "import", "data", "code" to sustain the project properly.
 
Then, 
we downladed the scores.csv file. 

As the following, 
we defined a list named HW_questions to compare the 
content of the students' questions and the actual homework's questions. We prepared a graph to show the
relation between the actual questions and student's questions.

After that,
due to we will continue with a common dataframe, we created a combined_df and we merged the questions_df and scores_df into the combined_df.

Then, 
in the following code snippet, 
we made another merge which is aggregated_texts and score_df to show represent each student in a single row. 

Then,
we applied tf/idf vectorizer, this is the beginning of data progressing.
 
In the following, 
we applied cosine similarity and jaccard similarity. As all the similarites are calculated for each question,
We decided to calculate the average for each student. 

Then, 
we shaped the combined_df in code - text- cosine similarity(Average)-jaccard similarity(Avg). For not missing any data we filled nan values. 

Plus,
To calculate our project's progress we applied random forest regression and we calculated the error values. 

After that, 
we applied the randomized search to develop our project and decrease the mse value where X = cosine similarity and Jaccard similartiy and Y = grade. Also, we splitted to X_train, X_test, y_train, y_test. The mse value decreased succesfully.

In the following code snippets, 
We represented the each student's error.
tables to show distribution of actual vs predicted grades.
Two trees (content is same) to visualize random forrest regression.
Representation of top words distrivuted by the letter grades.


As all the group members we worked on the project together with different duties.

Özen and Meltem mostly worked on the lectures and decided which methdos can be used and data representations' coding part.
Hakkı, Arda and Berdan we mostly worked on coding the decided methods.
 
