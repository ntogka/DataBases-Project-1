# DataBases
Ένα project με βάση στο AWS RDS δεσμεύοντας ένα μηχάνημα στο AWS με εγκατεστημένη postgreSQL. Δουλεύτηκε μέσω pgAdmin4

V.1

Σκοπός:

Φτιάχτηκε μια βάση δεδομένων για την αποθήκευση και εξερεύνηση δεδομένων που προέρχονται από την Airbnb. Η βάση δεδομένων αποτελείται από μία συλλογή πινάκων και τις μεταξύ τους
σχέσεις.Για να οριστεί το σχήμα της βασίστηκα στη μορφή των δεδομένων εισόδου, το οποίο απεικονίστικε σε ένα διάγραμμα ER.
Δημιουργήθηκαν πίνακες χρησιμοποιώντας SQL και θα εισάχθηκαν δεδομένα σε αυτούς με την εντολή \copy. Επίσης, δημιουργήθηκαν περιορισμοί ξένου κλειδιού για αναφορική ακεραιότητα.

Δεδομένα:
https://drive.google.com/open?id=1mrrXKz3RusWOUrhR0ap8nb2G2elIAjXz

Τι φτιάχτηκε:

● Ένα διάγραμμα ER με τους Airbnb πίνακες, τις σχέσεις και τις ιδιότητές τους.
● Τη βάση δεδομένων Airbnb σε ένα Postgres Cloud instance.
● Η βάση αυτή θα πρέπει να περιέχει πίνακες για τους οποίους θα ισχύουν τα εξής:
○ κάθε πίνακας να αντιστοιχεί σε ένα αρχείο .csv του Airbnb dataset.
○ να έχουν εισαχθεί σε αυτόν τα αντίστοιχα δεδομένα.
○ να περιέχει περιορισμούς πρωτεύοντος και/ή ξένου κλειδιού.

Tip:

Επειδή μερικές εντολές create table έχουν πολλά πεδία, όπως αυτή για τον πίνακα Listing, τρέχω το python πρόγραμμα gen_ddl_python3.py, το οποίο παίρνει ως παράμετρο το .csv αρχείο
των δεδομένων, π.χ. listings.csv για τον πίνακα Listing, και παράγει ένα αρχείο .sql με την εντολή create table για τον αντίστοιχο πίνακα. 


V.2

Σκοπός:

Εξερεύνηση δεδομένων του Airbnb με ερωτήματα σε SQL

Τι φτιάχθηκε:

● 12 SQL ερωτήματα που θα περιλαμβάνουν inner join, outer join, where,
order by, group by, limit, καθώς και χρησιμοποίηση των συναρτήσεων min,
max, avg, της λέξης κλειδί distinct, καθώς και χρησιμοποίηση των τελεστών
σύγκρισης like, between.
● Κάθε ερώτημα θα πρέπει να συνοδεύεται από μια μικρή περιγραφή που θα εξηγεί ποιος
είναι ο σκοπός του δηλαδή τι ζητάμε. Επίσης θα συνοδεύεται και από το πλήθος των
εγγραφών που επεστράφησαν ως αποτέλεσμα.
● Κάθε πίνακας εκ των Calendar, Listings, Reviews, Neighbourhoods, Geolocation θα
πρέπει να χρησιμοποιηθεί σε τουλάχιστον ένα ερώτημα.
● Τουλάχιστον 8 ερωτήματα θα πρέπει να περιέχουν ένα τουλάχιστον join.
● Τουλάχιστον 2 ερωτήματα θα πρέπει να περιέχουν ένα τουλάχιστον outer join


V.3
