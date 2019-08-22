# Online Book Shop Portal

## Tables

#### Table 1: categories
| sno | name | 
| --- | --- |
| 1 | Technical |
| 2 | Exam |



#### Table 2: books
| sno | name | price | published_date | category_id | active | 
| --- | ---  | --- | --- | -- | ---| 
| 1 | Java | 300 | 01-01-2011 | 1 | 1 | 
| 2 | JavaEE | 500 | 01-05-2019 | 1 | 1 |
| 3 | C | 100 | 01-06-2013 |1 | 0 | 
| 4 | MFCS | 100 | 01-06-2013 | 2 | 1 |


#### Table 3: users
| sno | name | 
| --- | --- |
| 101 | Naresh |
| 102 | Prabhu |

#### Table 4: orders

| sno | book_id |  user_id | quantity | 
| --- | --- | --- | --- | 
| 1 | 1 | 101 | 2 | 
| 2 | 2 | 102 | 1 |
 
 #### Table 5: book_ratings
 
| sno | book_id |  user_id | rating | 
| --- | --- | --- | --- | 
| 1 | 1 | 101 | 2 |
| 2 | 2 | 102 | 1 |

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
