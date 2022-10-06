Video URL : https://drive.google.com/file/d/1BWcP68pb8DxC9oy5EMWKKMzKANvMlSp2/view?usp=sharing


NOTES :

Normalization is a process of organizing the data in db to avoid the redundency(duplication).

Problems with data redundency:
1. Insertion, updation, deletion anomalies
2. Inconsistnecy of DB
3. Increase the DB table size and slow the performance while fetching the data.

In Normalization we should split a table in multiple tables so that each table should contains a single idea/concept.

To normaize a table we have diff types of normal forms:

1. 1NF 
2. 2NF 
3. 3NF-----> upto 3NF data redundency is almost minimized or removed
4. BCNF
5. 4NF
6. 5NF


First Normal Form:
- Each cell should contains only atomic value
- A table should not have the repeating columns.


Second Normal Form:
- Table must be in 1NF 
- Table must not contains any partial dependency

If the proper subset of a candidate key determines non-prime attribute, then it 
is called Partial Dependency.


Third Normal Form:
- Table should be in 2NF.
- There should not be any Transitive Dependency.

