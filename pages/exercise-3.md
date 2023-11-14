# Exercise 3: Templated Pages

Templated pages allow you to generate many pages from a single markdown file.

Each page has a different URL, but the same structure. The URL you use determines which content is displayed.

## a. Create a templated page file

_Exercise: Create a [templated page](https://docs.evidence.dev/core-concepts/templated-pages/) file that will display data for a particular item._

<Alert status="info">

**Hint:** To create a templated page, you need to surround the filename in square brackets, e.g. `pages/[item].md`.
</Alert>

## b. Access the item name in the templated page

_Exercise: Add the syntax to [display the selected item name](https://docs.evidence.dev/core-concepts/templated-pages/#using-page-parameters) on the page, and test it works by navigating to the page._

<Alert status="info">

**Hint:** Every templated page has access to the name of the variable you pass in the URL. If your templated page was called `[customer].md` then your would access the customer name using `{$page.params.customer}`.
</Alert>



You can test if your syntax is working by adding a test value to your URL locally. For example, `localhost:3000/customer/Acme` would display `Acme` on the page.

## c. Add navigation links

_Exercise: [Create links](https://docs.evidence.dev/core-concepts/templated-pages/#generating-templated-pages) to each of the item pages from this page._

Because Evidence builds website pages ahead of time, it needs to know all the templated pages you want to create.

In order to do that, it crawls the app and follows any links it finds.

<Alert status="info">

**Hint:** It is normally easiest to generate links using a query.
</Alert>

## d. Create content for the templated page

_Exercise: Create a component which displays [only data for the relevant item](https://docs.evidence.dev/core-concepts/templated-pages/#using-page-parameters)._

When using templated pages, you typically want to filter the data displayed in components.

Do this by filtering data before you pass it to a component.

<Alert status="info">

**Hint:** If you wanted to filter a particular customer, you would use: 
```javascript
data={customers.filter(d => d.customer_name === $page.params.customer)}
```
</Alert>