# RxTerms-PostgreSQL

RxTerms Download Page [**link**](https://wwwcf.nlm.nih.gov/umlslicense/rxtermApp/rxTerm.cfm).

## About

Scripts to create your own RxTerms Current Prescribable Content database for PostgreSQL.

## Releases

For full database creation, see [Releases](https://github.com/ZionDials/RxTerms-PostgreSQL/releases). The releases are only for the SQL creation file and contain **no Data files whatsoever**.

## Warning

As you should always have a primary key with any SQL database, whether it be auto generated or composite, I have used `RXCUI` as the Primary Key (And respective unique constraint) and it works perfectly fine. `RXCUI` as a Primary Key also helps when using this database with another database such as that for [RxNorm](https://github.com/ZionDials/RxNorm-PostgreSQL).

---

## Folder Structure

### Constraints  ( _constraints.sql )

The primary keys for each table in their respective SQL file.

### Indexes   ( _indexes.sql )

The unique and RxTerms recomended indexes for each table in their respective SQL file.

### Scripts ( RxTermsCurrentPostgreSQLDB.sql )

Contains the Full Database Creation `RxTermsCurrentPostgreSQLDB.sql`. This will create a database `RxTerms`. Then create all tables, indexes, and constraints in the `Public` schema.

### Tables ( _table.sql )

The table only creation scripts.