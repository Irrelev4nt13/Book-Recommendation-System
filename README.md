# Book-Recommendation-System
📚A book recommendation and classification system as well as a simple image retrieval system, using the Goodreads dataset.

## Data Cleaning and Preprocessing:

Our project begins by loading data from a CSV file named "books_1.Best_Books_Ever.csv." In this initial step, we focus on preparing the data for analysis.
1.  Converting BookId to Integers: We extract the "bookId" column and convert its values into integers. This step ensures that we can work with this essential identifier in numerical form.
2.  Handling Missing Values: We carefully handle missing values in specific columns. Rows with missing data are dropped to ensure the integrity of our dataset.
3.  Genre and Author Preprocessing: To facilitate further analysis, we preprocess genres and authors. This may involve tokenization, stemming, or other text processing techniques as required.

## Data Analysis:

With our cleaned and preprocessed dataset, we delve into data analysis, uncovering various insights and statistics:
1.  Descriptive Statistics: We calculate key statistics such as mean, median, and standard deviation for relevant attributes, providing an overall snapshot of the dataset.
2.  Histograms: To visualize the data distribution, we create histograms. In particular, we examine book ratings and page counts to understand their distributions.

## Recommendation System:

For this phase, we employ a recommendation system that leverages bigrams and unigrams:
1.  TF-IDF Vectorization: To represent textual data, we use TF-IDF (Term Frequency-Inverse Document Frequency) vectorization for both unigrams and bigrams. This technique assigns importance scores to words and word pairs based on their frequency.
2.  Cosine Similarity: We calculate cosine similarities between book descriptions. This measure quantifies the similarity between books based on their textual content.
3.  Book Recommendations: Using the calculated cosine similarities, we provide book recommendations. Users can input a book, and our system will suggest similar books based on textual content.

## Classification:

In this section, we explore classification tasks using Random Forest, Naive Bayes, and Support Vector Machines (SVMs):
1.  Textual Data Preprocessing: We preprocess textual data using techniques like glove to convert text into numerical features that can be used for classification.
2.  Classification Algorithms: We apply Random Forest, Naive Bayes, and SVC to classify books into predefined categories or labels. Each algorithm is evaluated separately.
3.  Performance Metrics: We evaluate the model performance using standard metrics such as precision, recall, F1-score, and accuracy. These metrics provide insights into how well the classifiers perform in assigning books to their respective categories.

## Image Retrieval System:

At least, we are going to build an Image retrieval System which will also recommends book based on the similarity between the images.
1.  Utilizes book cover images for visual search and retrieval.
2.  Implements image similarity algorithms to find visually similar books.
3.  Enhances the user experience with visually appealing book recommendations.
