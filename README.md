# ΒΔ

## Ορισμοί

**Βάση δεδομένων (ΒΔ - database DB)** είναι *μια συλλογή από σχετιζόμενα δεδομένα*. Παραδείγματα: Τηλεφωνικός κατάλογος, κατάλογος στοιχείων μαθητών κλπ.

**Σύστημα διαχείρισης βάσεων δεδομένων (ΣΔΒΔ - Database Management System DBMS)** είναι μια συλλογή από προγράμματα τα οποία επιτρέπουν στους χρήστες να δημιουργήσουν και συντηρήσουν μια ΒΔ.

Οι τρεις κύριες λειτουργίες που παρέχει ένα ΣΔΒΔ για τις ΒΔ είναι:

- Ο ορισμός (definition) μιας ΒΔ, δηλαδή ο καθορισμός των τύπων, δομών και περιορισμών των δεδομένων της βάσης.
- Η κατασκευή (construction) μιας ΒΔ, δηλαδή ο τρόπος μέσω του οποίου τα δεδομένα αποθηκεύονται στο δίσκο.
- Ο χειρισμός (manipulation) μιας ΒΔ, δηλαδή η υποβολή ερωτημάτω, εισαγωγή / επεξεργασία των δεδομένων κλπ.

*ΒΔ + ΣΔΒΔ = Σύστημα Βάσης Δεδομένων ΣΒΔ (Database System DBS)*

## Παράδειγμα

Βάση δεδομένων **ΣΧΟΛΗ**

- ΦΟΙΤΗΤΗΣ
- ΜΑΘΗΜΑ
- ΔΙΔΑΣΚΑΛΙΑ
- ΒΑΘΜΟΛΟΓΙΑ

## Διαφορές ΒΔ από απλά αρχεία / προγράμματα

- Αυτοπεριγραφική φύση: Εκτός από τα δεδομένα περιέχεται και η περιγραφή αυτών (*μετα-δεδομένα*) πχ δομή του αρχείου, τύποι δεδομένων, περιορισμοί επί των δεδομένων.
- Απόμονωση μεταξύ προγραμμάτων και δεδομένων: Μπορεί να γίνουν αλλαγές στη μορφή των δεδομένων χωρίς να χρειάζονται αλλαγές στα προγράμματα προσπέλασης.
- Πολλαπλές όψεις των δεδομένων: Κάθε χρήστης που χρησιμοποιεί τη ΒΔ δύναται να βλέπει μιά διαφορετική όψη των περιεχομένων της (πχ να μη βλέπει κάποια δεδομένα τα οποία δε του χρειάζονται)
- Υποστήριξη πολλαπλών χρηστών: Πολλοί χρήστες μοιράζονται τα δεδομένα μιας ΒΔ και μπορούν ταυτόχρονα να ενεργούν σε αυτά.

## Ωφέλη από τη χρήση ενός ΣΔΒΔ

- Μόνιμη αποθήκευση δεδομένων: Τα προγράμματα χρησιμοποιούν τις βάσεις δεδομένων για να αποθηκεύουν τα δεδομένα τους.
- Ευελιξία στα προγράμματα: Μπορεί εύκολα να γίνει αλλαγή στη μορφή μιας Βάσης Δεδομένων χωρίς να επηρεαστούν τα προγράμματα που την χρησιμοποιούν
- Ταχύτερη ανάπτυξη προγραμμάτων: Αντί το κάθε πρόγραμμα να χρησιμοποιεί το δικό του τρόπο για να αποθηκεύει τα αρχεία του, όλα χρησιμοποιούν τη Βάση Δεδομένων
- Έλεγχος πλεονασμών: Δε χρειάζεται κάθε χρήστης των δεδομένων να διατηρεί ξεχωριστό αρχείο - η βάση δεδομένων είναι κοινή απλώς κάθε ένας βλέπει τα δεδομένα που τον αφορούν.
- Περιορισμοί ορθότητας: Μπορούν να επιβληθούν περιορισμοί ώστε να διασφαλιστεί η ορθότητα των στοιχείων που γράφονται στη ΒΔ, πχ τύποι δεδομένων, συσχετίσεις μεταξύ εγγραφών κλπ
- Περιορισμός μη εξουσιοδοτημένης πρόσβασης: Κάθε χρήστης βλέπει τα δεδομένα που τον αφορούν και μόνον αυτά.
- Πολλαπλές διεπαφές χρήστη: Τα δεδομένα είναι κοινά αλλά μπορεί να υπάρχουν πολλές διεπαφές (interfaces) μέσω των οποίον τα βλέπουν οι χρήστες
- Παροχή μηχανισμών τήρησης εφεδρικών αντιγράφων και ανάκαμψης.

## Ταξινόμηση ΣΔΒΔ

Χρησιμοποιούνται διάφορα κριτήρια:

- Ανά μοντέλο δεδομένων
  - Σχεσιακό (Relational): Το πιο δημοφιλές μοντέλο, τα περισσότερα ΣΔΒΔ βασίζονται σε αυτό. Ουσιαστικά παριστάνει μια ΒΔ ως μια συλλογή από πίνακες.
  - Μη σχεσιακό (Non-Relation, NoSQL): Περιλαμβάνει διάφορα μοντέλα δεδομένων - παρότι μη σχεσιακές βάσεις υπήρχαν αρχικά, πριν την χρησιμοποίηση του σχεσιακού μοντέλου, έχει ξαναγίνει δημοφιλές τα τελευταία χρόνια λόγω της ευκολίας που δίνει στην οριζόντια κλιμάκωση (horizontal scaling - αντίθετα οι σχεσιακές ΒΔ κλιμακώνονται συνήθως κάθετα - vertical scaling). Ορισμένα μοντέλα δεδομένων μη σχεσιακών ΣΔΒΔ:
      - Key-value stores
      - Document-oriented


- Ανά αριθμό χρηστών:
  - Ενός χρήστη (single-user)
  - Πολλαπλών χρηστών (multi-user)


- Ανά αριθμό εγκαταστάσεων
  - Συγκεντρωτικά (centralized)
distributed)


- Ανοιχτού ή κλειστού κώδικα
- Γενικού ή ειδικού σκοπού


## Ορισμένα γνωστά ΣΔΒΔ

- Ανοιχτού κώδικα
  - Sqlite (relational / single-user / centralized )
  - Mysql (relational / multi-user / συνήθως centralized)
  - Postgresql (relational / multi-user / συνήθως centralized)
  - Postgresql (relational / multi-user / συνήθως centralized )
  - Redis (non relational -- key-value store / multi-user / συνήθως distributed )
  - Mongodb (non relational -- document-oriented / multi-user / συνήθως distributed )  


- Κλειστού κώδικα
  - Microsoft Access (relational / single-user / centralized)
  - Microsoft SQL Server (relational / multi-user / συνήθως centralized)
  - Oracle (relational / multi-user / συνήθως centralized)
  - IMB DB2 (relational / multi-user / συνήθως centralized)

# Το μοντέλο οντοτήτων συσχετίσεων

Το μοντέλο Οντοτήτων Συσχετίσεων (ΟΣ - Entity Relationship ER) χρησιμοποιείται
για την υψηλού επιπέδου αναπαράσταση δεδομένων. Κάθε αντικείμενο που θέλουμε
να αναπαραστήσουμε στη βάση ονομάζεται Οντότητα (entity πχ σπουδαστής, σχολή)
και έχει μια σειρά από γνωρίσματα/ιδιότητες (attributes πχ όνομα, ηλικία). Οι
αλληλεπιδράσεις μεταξύ των οντοτήτων είναι οι συσχετίσεις τους (relashinships
  πχ ο σπουδαστής φοιτά σε σχολή).

## Τύποι οντοτήτων

Ένας τύπος οντοτήτων είναι ένα σύνολο από οντότητες με τα ίδια γνωρίσματα
(προσοχή όχι με τις ίδιες τιμές στα γνωρίσματα) και αναπαρίσταται στο ΟΣ
διάγραμμα με ένα παραλληλόγραμμο. Τα γνωρίσματα του είναι ελλείψεις που
συνδέονται με ευθεία γραμμή με τον τύπο οντότητας, ενώ τα πλειότιμα
γνωρίσματα παρουσιάζονται με ελλείψεις με διπλό περίγραμμα.
Τα γνωρίσματα μπορεί να είναι:

- Απλά ή σύνθετα (όνομα / ονοματεπώνυμο)
- Μονότιμα ή πλειονότιμα (χρώματα ρούχου)
- Αποθηκευμένα ή παραγόμενα (ημ. γέννησης / ηλικία)
- Null (δεν έχει τηλέφωνο ή δε ξέρουμε τον αρ. τηλεφώνο)

Τα απλά γνωρίσματα παίρνουν τιμές από το πεδίο ορισμού τους.


Ένας τύπος οντοτήτων μπορεί να έχει κάποιο γνώρισμα το οποίο
έχει διακεκριμμένες τιμές για κάθε ξεχωριστή οντότητα. Το συγκεκριμένο
γνώρισμα μπορεί να χρησιμοποιηθεί για να προσδιορίσει μια οντότητα
(πχ ΑΤ φοιτητή)
και λέγεται γνώρισμα-κλειδί. Μπορεί να χρειάζονται παραπάνω από ένα γνώρισμα
για να προσδιοριστεί μοναδικά ένας τύπος οντοτήτων (πχ ΑΜ φοιτητή / σχολή που φοιτά)
τότε το σύνθετο γνώρισμα αυτό είναι το γνώρισμα-κλειδί του τύπου οντοτήτων.

## Τύποι συσχέτισης

Ένας τύπος συσχέτισης (relationship type) μεταξύ n τύπων οντοτήτων ορίζει
ένα σύνολο συνδέσεων / συσχετίσεων μεταξύ αυτών και αναπαραίσταται με ένα
ρόμβο που συνδέεται τους σχετιζόμενους τύπους οντοτήτων. Συνήθως οι τύποι
συσχέτισης συνδέοουν δύο οντότητες (είναι δηλαδή βαθμού δύο - δυαδικοί) πχ
ο τύπος συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ των ΕΡΓΑΖΟΜΕΝΟΣ και ΤΜΗΜΑ. Ένα παράδειγμα
τύπου συσχέτισης βαθμού τρία (τριαδικός) είναι ο τύπος συσχέτισης ΠΡΟΜΗΘΕΥΕΙ
μεταξύ των ΠΡΟΜΗΘΕΥΤΗΣ, ΑΝΤΙΚΕΙΜΕΝΟ, ΕΤΑΙΡΕΙΑ.

Ένα γνώρισμα μπορεί να θεωρηθεί ως συσχέτιση: Παράδειγμα το γνώρισμα ΚΩΔ_ΤΜΗΜΑΤΟΣ
του ΕΡΓΑΖΟΜΕΝΟΣ ή το (πλειότιμο) γνώρισμα ΕΡΓΑΖΟΜΕΝΟΙ του ΤΜΗΜΑ (το ένα είναι
αντίστροφο του άλλου) μπορούν να αναπαραστήσουν τον τύπο συσχέτισης ΕΡΓΑΖΕΤΑΙ.

Οι τύποι οντοτήτων που συμμετέχουν σε ένα τύπο συσχέτισης παίζουν ένα
συγκεκριμένο ρόλο (role). Για παράδειγμα, στον τύπο συσχέτισης ΕΡΓΑΖΕΤΑΙ
οι ρόλοι είναι οι εργαζόμενος (ΕΡΓΑΖΟΜΕΝΟΣ )και ο εργοδότης (ΤΜΗΜΑ). Οι ρόλοι
κυρίως έχουν σημασία σε αναδρομικούς τύπους συσχετίσεων (δηλαδή όταν ο ίδιος
τύπος οντοτήτων συμμετέχει περισσότερες από μία φορά σε ένα τύπο συσχετίσεων).
Για παράδειγμα ο τύπος συσχετίσης ΕΠΙΒΛΕΠΕΙ συσχετίζει τον τύπο οντοτήτων
ΕΡΓΑΖΟΜΕΝΟΣ με τον εαυτό του, μια φορά με το ρόλο προϊστάμενος και μια ακόμα
με το ρόλο υφιστάμενος.

Ο λόγος πληθικότητας για δυαδικές συσχετίσεις (cardinality ratio) προσδιορίζει
τον αριθμό των στιγμιοτύπων μιας συσχέτισης στα οποία μπορεί να συμμετέχει μια οντότητα.
Οι συνήθεις λόγοι πληθικότητας είναι 1:1, 1:Ν, Ν:1 και Μ:Ν. Παραδείγματα:

  - Ο τύπος συσχέτισης ΕΡΓΑΖΕΤΑΙ μεταξύ ΤΜΗΜΑ και ΕΡΓΑΖΟΜΕΝΟΣ έχει λόγο πληθικότητας 1:Ν (ήτοι ένα τμήμα έχει πολλούς εργαζόμενος αλλά ένας εργαζόμενος εργάζεται σε ένα μόνον τμήμα)
  - Ο τύπος συσχέτισης ΑΠΑΣΧΟΛΗΣΗ μεταξύ του ΕΡΓΑΖΟΜΕΝΟΣ και ΕΡΓΟ έχει λόγο πληθικότητα Μ:Ν (ήτοι ένας εργαζόμενος συμμετέχει σε πολλά έργα αλλά και ένα έργο υλοποιείται από πολλούς εργαζόμενους)
  - Ο τύπος συσχέτισης ΔΙΕΥΘΥΝΕΙ μεταξύ του ΕΡΓΑΖΟΜΕΝΟΣ και ΤΜΗΜΑ είναι 1:1 (ήτοι ένα τμήμα έχει ένα διευθυντή και ένας εργαζόμενος μπορεί να διευθύνει ένα τμήμα)


Οι τύποι συσχετίσεων μπορεί και αυτοί να έχουν γνωρίσματα. Για παράδειγμα
στον τύπο συσχέτισης ΑΠΑΣΧΟΛΗΣΗ μπορεί να περιλάβουμε ένα γνώρισμα ώρες για
τις ώρες που συμμετείχε ο ΕΡΓΑΖΟΜΕΝΟΣ στο ΕΡΓΟ. Άλλο παράδειγμα είναι το γνώρισμα
ημερομηνία έναρξης για τον τύπο συσχέτισης ΔΙΕΥΘΥΝΕΙ. Τα γνωρίσματα των 1:1 ή
1:Ν τύπων συσχετίσεων μπορούν να μεταφερθούν σε έναν από τους συμμετέχοντες
τύπους. Για παράδειγμα το ημερομηνία έναρξής μπορεί να είναι γνώρισμα είτε του
ΕΡΓΑΖΟΜΕΝΟΣ είτε του ΤΜΗΜΑ (καλύτερα όμως στο ΤΜΗΜΑ - γιατί;). Για τους 1:Ν
τύπους συσχετίσεων το γνώρισμα μπορεί να μεταφερθεί μόνον στην πλευρά του Ν,
για παράδειγμα, στη στον τύπο συσχετίσης ΕΡΓΑΖΕΤΑΙ, το γνώρισμα ημερομηνία
έναρξης μπορεί να μεταφερθεί μόνον στην πλευρά του ΕΡΓΑΖΟΜΕΝΟΣ (και όχι στο
ΤΜΗΜΑ - γιατί; ). Το γνώρισμα ώρες όμως του Μ:Ν τύπου συσχετίσεων ΕΡΓΟ
δε μπορεί να μεταφερθεί σε κανένα τύπο οντοτήτων.

Παράδειγμα:

                    -
                   /--  ΕΡΓΑΖΕΤΑΙ -\
     ΕΡΓΑΖΟΜΕΝΟΣ -/                 \ - ΤΜΗΜΑ
        |  |      \                 /      |
        |  |       \--  ΔΙΕΥΘΥΝΕΙ --/    ΕΛΕΓΧΕΙ
     ΕΠΙΒΛΕΨΗ       \                      |
                     \                     |
                     ΑΠΑΣΧΟΛΗΣΗ ------ ΕΡΓΟ



# Το σχεσιακό μοντέλο δεδομένων

Στο σχεσιακό μοντέλο η ΒΔ είναι μια συλλογή από πίνακες τους οποίους στο εξής θα ονομάζουμε **σχέσεις (relations)**. Κάθε "γραμμή" της σχέσης παριστάνει μια συλλογή από σχετιζόμενες τιμές δεδομένων και ονομάζεται **πλείαδα (tuple)**. Η επικεφαλίδα κάθε "στήλης" της σχέσης ονομάζεται **ιδιότητα (attribute)** ενώ ο τύπος των δεδομένων που μπορεί να έχει κάθε "στήλη" ονομάζεται **πεδίο ορισμού (domain)**.

Μια σχέση περιγράφεται από το **σχήμα σχέσης (Relation schema) R** το οποίο μπορεί να δηλωθεί ως *R(A<sub>1</sub>,A<sub>2</sub>, ..., A<sub>n</sub>)* με το R να είναι το όνομα της σχέσης και Α οι ιδιότητες της. Παράδειγμα, η σχέση ΣΠΟΥΔΑΣΤΗΣ(Αρ. μητρώου, όνομα, ημ. γέννησης, τηλέφωνο, email). Ο αρ. ιδιοτήτων μιας σχέσης ονομάζεται και **βαθμός της σχέσης (degree of a relation)** πχ η σχέση ΣΠΟΥΔΑΣΤΗΣ είναι βαθμού 5.

Μια σχέση τώρα (δηλαδή μια κατάσταση/στιγμιότυπο) του σχήματος σχέσης R είναι ένα σύνολο από πλειάδες r = {t<sub>1</sub>, t<sub>2</sub>, ..., t<sub>m</sub>} με κάθε πλειάδα t να είναι ένα σύνολο από n τιμές t = &lt;v<sub>1</sub>, v<sub>1</sub>, ..., v<sub>n</sub>&gt;

σ<sub>⋈</sub> &220;
⋈


s<sub>s</sub>




| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
