# W5D2 - Database Design

### To Do
- [x] Primary Keys/Foreign Keys
- [x] Data Types
- [x] Relationship Types
- [x] Naming Conventions
- [x] Normalization
- [x] Design Concepts
- [x] Entity Relationship Diagrams
- [x] Breakout: Convert 2 Spreadsheets [20 mins]
- [x] Student Suggestion ERD(s)

### Primary Keys
* uniquely identifying a record in a table
* MUST be unique
* Auto-incrementing integer
* Foreign key's data type MUST MATCH the PK's
* Composite keys (try to avoid)

### Data Types
* Used to be a big concern
* Storage is now cheap!!
* integer
* varchar(255)
* boolean
* postal codes H0H 0H0 <-- string, '00215'
* 555-555-5555 (555)555-5555 555555555 <--- string

### Relationships
* One-to-One: one record in the first table is related to only one record in the 2nd
* One-to-Many: one record in the 1st table is related to zero or more in the 2nd
* Many-to-Many: many records in the 1st related to many records in the 2nd

### Naming Conventions
* Always opinionated/liable to change
* table names and field names are `snake_case`
* You can use spaces BUT DON'T "first name"
* Table names are always plural
* Primary keys just call 'em `id`
* Foreign keys singular table name plus `_id` user_id, tweet_id

### Normalization
* 1NF, 2NF, 3NF
* Refactor to reduce redundancy
* Single source of truth
SUM(line_items.price)
* Try to avoid storing calculated fields
first_name, last_name, full_name
* Beware: this process can be taken too far

### Design Concepts
* Required fields: the status of the record at initial save
* Default: timestamps `created_at` default to NOW(), use intelligent defaults to make thing easier
* Pull repeating out to their own table: lookup tables
* <select>
* Try not to delete anything, use an `active` boolean, default to `true`

ALTER TABLE

Calgary, Cal, Cagary, calgary, cow town
2 - Calgary
3 - Toronto

### ERD
* Entity Relationship Diagrams




### Breakout: Convert Two Spreadsheets
- [Gist with instruction](https://gist.github.com/andydlindsay/20e7305e853bad7b587f294b054cf8de)



### Useful Links
* [Database Normalization](https://en.wikipedia.org/wiki/Database_normalization)
* [Postgres Data Types](http://www.postgresqltutorial.com/postgresql-data-types/)
* [Relationship Types](http://etutorials.org/SQL/Database+design+for+mere+mortals/Part+II+The+Design+Process/Chapter+10.+Table+Relationships/Types+of+Relationships/)
* [draw.io (online ERD)](https://www.draw.io/)