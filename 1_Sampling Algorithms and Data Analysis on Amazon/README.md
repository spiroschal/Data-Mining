>EN
# Sampling Algorithms and Data Analysis on Amazon

**Question 2** requires you to analyze data from a file “data.csv” with three columns (A, B, C), where the values in columns B and C are functions of column A with added random noise. The task is to load the data, create plots that visualize the relationships between B and C with A, and then determine the type of function that connects these columns, e.g., whether it is logarithmic, polynomial, exponential, or another type.

**Question 3** requires you to perform exploratory data analysis on two files containing information on mobile phone products and their reviews on Amazon. The goal is to analyze the distribution of reviews per product, investigate the evolution of ratings over time, and explore the relationship between price and average rating. Additionally, it asks to investigate the difference in ratings across various brands and examine hypotheses regarding review helpfulness and verified purchases.

The following files are required:
1. **data.csv**: Used in Question 2. It contains three columns (A, B, C) with 1000 rows of data. The values in columns B and C are calculated as functions of column A, with added random noise.
2. **Cell_Phones_meta.csv**: Required for Question 3, this file contains metadata (such as price and brand) for mobile phone products. It is used to analyze relationships and hypotheses related to the characteristics of the products.
3. **Cell_Phones_and_Accessories_5.json**: Also used in Question 3, this file contains product reviews in JSON format. It includes reviews for products, with fields such as rating and date, and is used for analyzing ratings and the relationships that arise from them.

---
>GR
# Αλγόριθμοι Δειγματοληψίας και Ανάλυση Δεδομένων στην Amazon

Η **Ερώτηση 2** ζητά να αναλύσετε δεδομένα από ένα αρχείο “data.csv” με τρεις στήλες (A, B, C), όπου οι τιμές στις στήλες B και C είναι συναρτήσεις της στήλης A με την προσθήκη τυχαίου θορύβου. Ο στόχος είναι να φορτώσετε τα δεδομένα, να δημιουργήσετε γραφήματα που απεικονίζουν τις σχέσεις των B και C με το A, και στη συνέχεια να προσδιορίσετε τον τύπο της συνάρτησης που συνδέει τις στήλες, π.χ., αν είναι λογαριθμική, πολυωνυμική, εκθετική ή άλλου τύπου.

Η **Ερώτηση 3** ζητά να εκτελέσετε διερευνητική ανάλυση δεδομένων από δύο αρχεία με πληροφορίες για προϊόντα κινητών τηλεφώνων και τις αξιολογήσεις τους στην Amazon. Στόχος είναι να αναλυθεί η κατανομή των αξιολογήσεων ανά προϊόν, να εξεταστεί η σχέση των βαθμολογιών στον χρόνο και η σχέση της τιμής με τη μέση αξιολόγηση. Επίσης, ζητά να διερευνηθεί η διαφορά στις αξιολογήσεις μεταξύ διαφόρων εμπορικών σημάτων και να εξεταστούν υποθέσεις για τη χρησιμότητα των αξιολογήσεων και τις επιβεβαιωμένες αγορές.

Απαιτούνται τα εξής αρχεία:
1. **data.csv**: Χρησιμοποιείται στην Ερώτηση 2. Περιέχει τρεις στήλες (Α, Β, C) με 1000 γραμμές δεδομένων. Οι τιμές στις στήλες Β και C υπολογίζονται ως συναρτήσεις της στήλης Α, με προσθήκη τυχαίου θορύβου.
2. **Cell_Phones_meta.csv**: Απαιτείται για την Ερώτηση 3 και περιέχει μεταδεδομένα (όπως τιμή, μάρκα) για προϊόντα κινητών τηλεφώνων. Χρησιμοποιείται για να αναλυθούν οι σχέσεις και οι υποθέσεις σχετικά με τα χαρακτηριστικά των προϊόντων.
3. **Cell_Phones_and_Accessories_5.json**: Χρησιμοποιείται επίσης στην Ερώτηση 3 και περιέχει αξιολογήσεις προϊόντων σε μορφή JSON. Περιλαμβάνει κριτικές για προϊόντα, με πεδία όπως rating και ημερομηνία, και χρησιμοποιείται για την ανάλυση των βαθμολογιών και των σχέσεων που προκύπτουν από αυτές.
