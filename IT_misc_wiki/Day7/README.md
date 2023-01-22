<a href="https://github.com/tyomhk2015/book/tree/main/IT_misc_wiki" rel="noopener noreferrer"><b><< Back</b></a>

# Day 7

From chapter 30 to 34.



### Chapter 30

<b><i>COVID-19 and legacy system</i></b>

During pendemic I have seen an article about a company, or companies, desperately looking for COBOL engineers. Why didn't that company try to hire the retired COBOL experts that have willingness to do the job? Perhaps the company who were looking for COBOL developers did not try to pay sufficiently to the potention COBOL applicants, I guess.

There are some takeaways from the COBOL, or legacy system, incident mentioned above.

1. <b>The developer must be build an application with repsonsibilities.</b>

Moreover, I would like to add the 'core members' to the word 'developers'.
Depending on how they struct a program give huge difference when comes to maintaining the application after it is launched.

I recently participated a project that builds LINE MINI applications, and seen some code bases that are calling API requests more than necessary. By pursuading the core members of the project, reduced the API request calls from 3 to 1. Removing unncessary calls by 2 resulted alleviating server workload of handling the API requests by 66%, and improving the rendering speed on the client about 50% on average.

Not only core developers but also the directors or product managers should also take some responsibilities. From my experience, the quality, the difficulty of maintance and development is affected by the directors' order. Especially the ones that do not take even a look at the product, and the ones that switch the plans of the product very often without any convincing evidence.

2. <b>Programs should be maintained continuosly.</b>

The heads or the boards of companies do not take software program or product seriously. Perhaps they are only interested in money. If they were aware of the their own products, they may have invested some capital to maintain and stabilize their service, and prevent potiential lack of workers for operating the program.

It surely was shocked that the system administrator of the company, that was looking for COBOL, the one mentioned above, was not aware of the program's details that had been running for more than 20 years.

No matter what project you would participate in the future, making habit of figuring out what tech stack the project is running on would never hurt you.


### Chapter 31

<b><i>SQL</i></b>

- SQL: Structured Query Language

A language for communicating with `DBMS`(DataBase Management System) to manage `DB`(DataBase).

Learned that MySQL, PostgreSQL, MariaDB etc, are `DBMS`, not `DB`. `DB`, itself is just a storage that stores data. `DBMS` is the one that maintains and takes care of querying requests from developers. For the sake of convenience, people tend to call `DBMS` + `DB` as `DB`, but strictly speaking, they are separate entities.

Surprise to find that there are developer who are reluctant to studying SQL due to the developer experience that ORMs provide. Cannot deny that it lets developers save time, but it does not mean `ORM` substitutes the knowledge of `SQL`. This is just imagination, but when it comes to tuning the performace of querying, `ORM` may not be able to solve such problems solely.

By the way, `ORM`(Object relational mapping) is a tool that enables other languages to be translated to SQL commands.


### Chapter 32

<b><i>NOSQL</i></b>

Not Only SQL. Another type of SQL that is not constraint to relational database.
Some of famous NOSQL DBMSs are document DB, key-value DB, and graph DB.

1. Document DB

Data consist like an array filled with objects, just like JSON. It has some freedom in context of data types.

```
  data = [
    { "id": 1, "name": "Denzi" },
    { "id": 2, "name": "Makima" },
  ]
```
E.g. Mongo DB, firebase realtime DB, Amazon DocumentDB.

What is good about the document DB?

It helps the developer a new data without too much constraints compared to SQL. With SQL, to add a new data(row), the developer have designate `id`, and `name` specifically. If the values for properties(columns) are not provided, then there should be a hanlder that cares of the exceptions. This also applies when adding a new column to existing table. With NOSQL, you can omit some of columns and create a new data.

2. Key-value DB

Able toread/write more than 10K data in a second. Usually used for large scale data.

E.g. CassandraDB, DynamoDB (AWS), Redis

```

# setting a value for a key
  redis> SET mykey "my value"
  OK

# retrieving a value for a key
  redis> GET mykey
  "my value"

# deleting a key-value pair
  redis> DEL mykey
  (integer) 1
```

3. Graph DB

Uses `nodes` not columns or documents. `Node` means an individual data point or record in the graph, for instance a person, a store, place etc.

Graph DB are used for handling complex relationships with nodes, and Facebook uses the graph DB for their service.

There is no which one is the best or the worst, since the DBs mentioned above are for different purposes. Most of the time MySQL is sufficient for building applications, but if you need some perfomance improvement or need to build a specific feature, choose the DB that meets most of your application's requirement.

### Chapter 33

<b><i>Git and Github</i></b>

Git, a program that keeps track of how your files are changed and maintained.
Github, a cloud service that stores all the tracks that Git has made, and any collaborators can see the history of the changes.


### Chapter 34

<b><i>Versioning</i></b>

SemVer, Semantic Versioning Specification.

```
  v1.2.3
```

The first digit, 1, shows huge changes of the program.

The second digit, 2, shows minor changes of the program.

The third digit, 3, shows the number of bug fixes.

However, the versioning rule varies from projects to projects.

<hr>

 #노마드코더 #북클럽 #노개북