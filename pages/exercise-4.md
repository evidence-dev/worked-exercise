# Exercise 4: Templated Pages

[Templated pages](https://docs.evidence.dev/core-concepts/templated-pages/) generate many pages from a single markdown file. For example you can create a page for each product, category or customer in your database.

Each page has a different URL, but uses the same markdown file. The URL you use determines which content is displayed.

## a. Create a `queries` folder

_Exercise: Create a `queries` folder in the root of your project._

This stores queries that you can access in all your markdown files. Each file is named `query_name.sql`.

## b. Write a query returning one row for each page you want to create

_Exercise: Write a query and save it in the `/queries` folder._


## c. Scaffold the templated pages from the query

_Exercise: Run the `Evidence: Create Templated Page from Query` command in the command palette._

<Alert status="info">

**Hint:** Access the command palette with `Ctrl/Cmd + Shift + P`.
</Alert>

- This scaffolds out a new folder for you with an index page, and a templated page. 
- Once you've made it, go to the new page in the browser and test the links in the table.

## d. Customize the Content on your Templated Page

_Exercise: Add a metric or measure for the specific entity the page represents._
