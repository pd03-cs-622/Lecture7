## Databases

Benefits of XML/JSON over CSV/TSV: we can have hierarchies!

Why not just put all your data into a JSON? -> search and indexing is much faster

### Relational databases

Relies on schemas and pre-defined columns that data gets assigned to

**Transaction**: sequence of SQL operations that needs to all pass or if fails, rollback
- Prevents a failed operation in the middle of the unit of commands

Disadvantage of relational databases: no mapping between objects and table in between
- Not a hot topic anymore (30 years), no one likes doing this

#### Some history

Problem of enforcing schema:
- Makes data redundant, too much information
- NoSQL (not-just-sql) comes in! Document databases

Graph database is not used anywhere, not useful

Hierarchical database is anciety

#### How does it work

Relational database normalization

SQL is not good at dealing with many-to-many relationships

So convert to two "one-to-many" relationship:
- Instead of Student <> Course, we have Student <> Student Course <> Course
- Student Course has two foreign keys as a primary key (its a bridge table)

Sometimes normalization makes the database very complicated! Too many tables!

#### NoSQL / Document-based database

Talking about... one corporation (Oracle) literally owning everything

RIP NoSQL as an independent open-source program
- I guess NoSQL community open-source version exists

MongoDB most popular 

Does not enforce schema (its optional)

Go with a combination of document + relational database

No joint and complex operations

### Query languages

All types of databases need CRUD operations

Imperative vs. declarative queries: steps on how to get data vs. say what we want

#### Graph database

Data stored in nodes and vertices

Cypher, Neo4J (for property graph models)

Don't care about this concept, don't need to know it, its garbage

RDF: popular graph data structure as subject and connected to traits (by vertices)


