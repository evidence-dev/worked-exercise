# Exercise 1: Run queries and display results

The markdown code for this page is stored in `pages/exercise-1.md`.

This exercise is intended to be completed inside the markdown file.

## Sample data

This project is connected to a sample DuckDB database called `needful_things.duckdb`.


```sql information_schema
select
    table_name,
    column_name,
    data_type
from information_schema.columns
```

## a. Explore the database

_Exercise: Query the `orders` table, and return the results in a [DataTable component](https://docs.evidence.dev/components/data-table)._

<Alert status="info">

**Hint:** Try typing `/SQL` and pressing Tab to insert a query using slash command.
</Alert>

<!-- here is some space for your work -->

## b. Perform a calculation in SQL

_Exercise: Find the average order value across all orders._

<Alert status="info">

**Hint:** The column you want is called `sales`.
</Alert>

<!-- here is some space for your work -->

## c. Present the result in a BigValue component

_Exercise: Present the result of the previous query in a [BigValue component](https://docs.evidence.dev/components/big-value)._

<Alert status="info">

**Hint:** You can use slash commands to quickly insert components. Try typing `/bigvalue` and pressing Tab
</Alert>

<!-- here is some space for your work -->

When you're done, move onto [Exercise 2](/exercise-2).

<BigLink href="/exercise-2">Exercise 2 &rarr;</BigLink>
