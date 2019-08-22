# Online Book Shop Portal

## Tables

#### Table 1: books

| sno | name | price | published_date | category | active | rating |
| --- | ---  | --- | --- | -- | ---| -- |
| 1 | Java | 300 | 01-01-2011 | Technical | 1 | 4 |
| 2 | JavaEE | 500 | 01-05-2019 | Technical | 1 | 4| 
| 3 | C | 100 | 01-06-2013 |Technical | 0 | 2 |
| 4 | MFCS | 100 | 01-06-2013 | Exam | 1 | 5 |

#### Feature 1: Display All Books
`
select * from books where active = 1;
`

#### Feature 2: Display All Books - Sort by Price ASC
`
select * from books where active = 1  order by price asc;
`

#### Feature 3: Display All Books - Sort by Price DESC
`
select * from books where active = 1 order by price desc;
`

#### Feature 4: Display All Books - Based on Price Range
`
select * from books where active = 1 and price >= ? and price <= ? order by price asc;
`

#### Feature 5: Display All Books - Recently Published Books as First
`
select * from books order by published_date asc;
`

#### Feature 6: Display All Books - Based on the given category
`
select * from books where category = ?;
`


#### Feature 7: Display All Books - Based on the rating desc
`
select * from books where active = 1 order by rating desc;
`
