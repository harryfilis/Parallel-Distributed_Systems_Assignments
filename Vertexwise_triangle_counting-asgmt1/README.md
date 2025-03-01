
# Παράλληλα και Διανεμημένα Συστήματα
## Αποθετήριο 1ης Εργασίας - Vertexwise Triangle Counting
Description of the first assignment:
Given an adjacency matrix A in matrix market format, our code calculates in how many triangles is each node adjacent to. This is done using  method, namely V3 using a triple for loop .

* Κώδικας για το v1 : [triangle_v1.c](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/triangle_v1.c)
* Κώδικας για το v2 : [triangle_v2.c](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/triangle_v2.c)
* Για το ερώτημα-version 3 έχουμε:
  * [triangle_v3.c](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/triangle_v3.c)
  * [triangle_v3_cilk.c](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/triangle_v3_cilk.c)
  * [triangle_v3_openmp.c](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/triangle_v3_opmp.c)</br>
Όσον αφορα το 3.1 ο κώδικας που υλοποιήθηκε σε matlab είναι ο εξής
  * [3-1.m](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/3-1.m)
  
Tα αρχεία που δείχνουν την απόδoση του κώδικα (για του αντίστοιχους γράφους) σε παραλληλισμό είναι τα εξής png:
  * [belgium_v3.png](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/belgium_v3.png)
  * [cielskian_v3.png](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/cielskian_v3.png)
  * [dble_v3.png](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/dble_v3.png)
  * [NACA_v3.png](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/NACA_v3.png)
  * [youtube_v3.png](https://github.com/harryfilis/Parallel_and_Distributed_Systems_Assignments/blob/master/Vertexwise_triangle_counting-asgmt1/youtube_v3.png)
  
  Ο φάκελος matrices περιέχει όλους τους πίνακες που χρησιμοποιήθηκαν απο το Matrix Market</br>
  * readmtxfile.c ~ κώδικας που διαβάζει αρχείο πίνακα</br>
  * Makefile ~ Απαιτούμενο Makefile που κτιζει τα προγράματα και τα τρέχει.</br>
  * bashscript.sh ~ ShellScript που κάνει αυτόματα την δουλειά του testing.</br>
Ο φάκελος time περιέχει λίστες διαδοχικων τρεξιμάτων των τεστ με διαφορετικά numberOfWorkers πχ:
  ```js

  /triangle_v3_cilk ./matrixes/belgium_osm/belgium_osm.mtx 1 2 
  There are 2 workers.
  Matrix Loaded, now Searching!
  Sum: 1260 
  Duration: 0.018063 
  ``` 
  Η ανάλυση γίνεται στο αρχείο της αναφοράς.</br>
  Το μέρος v4 δεν έγινε λόγω έλλειψης χρόνου.</br>
  Συγγραφέας: Χάρης Φίλης ΑΕΜ:9449 email:charisfilis@ece.auth.gr </br>
