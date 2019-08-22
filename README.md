# Online Book Shop Portal

## Tables

#### Table 1: books

| sno | name | price | published_date | 
| --- | ---  | --- | --- |
| 1 | Java | 300 | 01-01-2011 |
| 2 | JavaEE | 500 | 01-05-2019 |
| 3 | C | 100 | 01-06-2013 |

#### Feature 1: Display All Books
`
select * from books;
`

#### Feature 2: Display All Books - Sort by Price ASC
`
select * from books order by price asc;
`

#### Feature 3: Display All Books - Sort by Price DESC
`
select * from books order by price asc;
`

#### Feature 4: Display All Books - Based on Price Range
`
select * from books where price >= ? and price <= ? order by price asc;
`

#### Feature 5: Display All Books - Recently Published Books as First
`
select * from books order by published_date asc;
`
