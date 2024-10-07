>EN
# Recommendation System Algorithms

**Step 1: Data Processing** In the first step, you process the cell_phone_ratings.csv file, keeping only users who rated more than 5 phones and phones rated by more than 5 users. You implement a pruning algorithm until these conditions are satisfied. In the end, you split the data into a training set (90%) and a test set (10%) and use the train.csv and test.csv files.

**Step 2: Implementation of UA and IA Algorithms** In this step, you implement the User Average (UA) and Item Average (IA) algorithms. UA predicts the average rating of a user, while IA predicts the average rating of a phone. You calculate the RMSE and report the results for both algorithms, using dataframes with pandas library commands.

**Step 3: Implementation of SVD** In the third step, you implement the Singular Value Decomposition (SVD) algorithm. You load the training dataset into a sparse matrix and calculate the rank-k approximative value of the matrix. You compute the RMSE for various values of k and create a plot of RMSE against k, mentioning the k value that achieves the minimum RMSE.

**Step 4: Implementation of UCF** In this step, you implement the User-Based Collaborative Filtering (UCF) algorithm. You again create the sparse matrix and compute ratings using the k nearest neighbors. You create a function that calculates ratings for a pair (u, c) and for various k values, recording the RMSE.

**Step 5: Implementation of ICF** In the fifth step, you implement the Item-Based Collaborative Filtering (ICF) algorithm, which is similar to UCF but focuses on columns instead of rows. You calculate the rating for each pair (u, c) using the k nearest items and record the RMSE.

**Step 6: Implementation of Cluster-Average** In the sixth step, you apply clustering using the k-means algorithm and calculate average ratings for users in each cluster. You test various k values and create graphical plots with the results. You report the outcomes of the algorithm.

**Step 7: Comparative Evaluation of Algorithms** After completing all previous steps, you conduct a comparative evaluation of all algorithms. You create a table listing the algorithms and their best achieved RMSE, commenting on the results.

The following files are required:
1. **cell_phone_ratings.csv**: This file contains the triples of reviewerID, asin, and overall representing user ratings for mobile phones. It is used for data processing and implementing the algorithms.

2. **cell_phone_ratings_pruned.csv**: This file contains the data after processing and pruning users and phones. You will find the triples that satisfy the conditions of the first step in this file.

3. **ratings_train.csv**: A file that contains 90% of the triples from the pruning and is used as the training set for training the algorithms.

4. **ratings_test.csv**: A file that contains 10% of the triples from the pruning and is used as the test set for evaluating the algorithms.

---
>GR
# Αλγόριθμοι Συστήματος Συστάσεων

**Βήμα 1: Επεξεργασία Δεδομένων** Στο πρώτο βήμα, επεξεργάζεστε το αρχείο cell_phone_ratings.csv, κρατώντας μόνο τους χρήστες που έχουν βαθμολογήσει περισσότερα από 5 κινητά και τα κινητά που έχουν βαθμολογηθεί από περισσότερους από 5 χρήστες. Υλοποιείτε έναν αλγόριθμο κλαδέματος μέχρι να ικανοποιούνται αυτές οι συνθήκες. Στο τέλος, διαχωρίζετε τα δεδομένα σε training (90%) και test set (10%) και χρησιμοποιείτε τα αρχεία train.csv και test.csv.

**Βήμα 2: Υλοποίηση Αλγορίθμων UA και IA** Σε αυτό το βήμα, υλοποιείτε τους αλγορίθμους User Average (UA) και Item Average (IA). Ο UA προβλέπει τη μέση βαθμολογία ενός χρήστη, ενώ ο IA τη μέση βαθμολογία ενός κινητού. Υπολογίζετε το RMSE και αναφέρετε τα αποτελέσματα για τους δύο αλγόριθμους, χρησιμοποιώντας dataframes με εντολές της βιβλιοθήκης pandas.

**Βήμα 3: Υλοποίηση SVD** Στο τρίτο βήμα, εφαρμόζετε τον αλγόριθμο Singular Value Decomposition (SVD). Φορτώνετε το training dataset σε έναν αραιό πίνακα και υπολογίζετε την rank-k προσεγγιστική τιμή του πίνακα. Υπολογίζετε το RMSE για διάφορες τιμές του k και δημιουργείτε γραφική παράσταση του RMSE ως προς το k, αναφέροντας την τιμή του k που επιτυγχάνει το ελάχιστο RMSE.

**Βήμα 4: Υλοποίηση UCF** Σε αυτό το βήμα, υλοποιείτε τον αλγόριθμο User-Based Collaborative Filtering (UCF). Δημιουργείτε ξανά τον αραιό πίνακα και υπολογίζετε τις βαθμολογίες χρησιμοποιώντας τους k πιο όμοιους χρήστες. Δημιουργείτε μια συνάρτηση που υπολογίζει τις βαθμολογίες για ένα ζευγάρι (u, c) και για διάφορες τιμές του k, και καταγράφετε το RMSE.

**Βήμα 5: Υλοποίηση ICF** Στο πέμπτο βήμα, υλοποιείτε τον αλγόριθμο Item-Based Collaborative Filtering (ICF), ο οποίος είναι παρόμοιος με τον UCF, αλλά εστιάζει σε στήλες αντί για γραμμές. Υπολογίζετε την βαθμολογία για κάθε ζευγάρι (u, c) χρησιμοποιώντας τους k πιο όμοιους αντικειμένων και καταγράφετε το RMSE.

**Βήμα 6: Υλοποίηση Cluster-Average** Στο έκτο βήμα, εφαρμόζετε clustering με τον αλγόριθμο k-means και υπολογίζετε τις μέσες βαθμολογίες για τους χρήστες σε κάθε cluster. Δοκιμάζετε διάφορες τιμές του k και δημιουργείτε γραφικά διαγράμματα με τα αποτελέσματα. Αναφέρετε τα αποτελέσματα του αλγόριθμου.

**Βήμα 7: Συγκριτική Αξιολόγηση Αλγορίθμων** Αφού ολοκληρώσετε όλα τα προηγούμενα βήματα, κάνετε μια συγκριτική αξιολόγηση όλων των αλγορίθμων. Δημιουργείτε έναν πίνακα με τους αλγορίθμους και το καλύτερο RMSE που επιτυγχάνει ο καθένας, σχολιάζοντας τα αποτελέσματα.

Απαιτούνται τα εξής αρχεία:
1. **cell_phone_ratings.csv**: Αυτό το αρχείο περιέχει τις τριάδες reviewerID, asin και overall που αναπαριστούν τις αξιολογήσεις χρηστών για κινητά τηλέφωνα. Χρησιμοποιείται για την επεξεργασία των δεδομένων και την υλοποίηση των αλγορίθμων.

2. **cell_phone_ratings_pruned.csv**: Αυτό το αρχείο περιέχει τα δεδομένα μετά την επεξεργασία και το κλάδεμα των χρηστών και των κινητών τηλεφώνων. Στο αρχείο αυτό θα βρείτε τις τριάδες που ικανοποιούν τις συνθήκες του πρώτου βήματος.

3. **ratings_train.csv**: Αρχείο που περιέχει το 90% των τριάδων από το κλάδεμα και χρησιμοποιείται ως training set για την εκπαίδευση των αλγορίθμων.

4. **ratings_test.csv**: Αρχείο που περιέχει το 10% των τριάδων από το κλάδεμα και χρησιμοποιείται ως test set για την αξιολόγηση των αλγορίθμων.
