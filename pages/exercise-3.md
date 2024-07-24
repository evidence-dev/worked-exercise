# Exercise 3: Loops and Conditional Logic

Here we're going to use Evidence features to iterate through data, and conditionally choose whether to display content.

## a. Write a query to get category sales

_Exercise: Write a query to return the category name and the total sales for that category._

<!-- here is some space for your work -->

## b. Create an `{#each}` loop

_Exercise: Write a [loop](https://docs.evidence.dev/core-concepts/loops) that displays the category name and the total sales for that category in a list._


<Alert status=info>

**Hint:** The syntax for loops is

```html
{#each query_name as row_alias}
    
Some content and data from rows {row_alias.column_name} 

{/each}
```
</Alert>

<!-- here is some space for your work -->


## c. Add an `{#if}` condition to the loop

_Exercise: Add an [if statement](https://docs.evidence.dev/core-concepts/if-else) inside the loop so that it only displays categories with sales greater than a particular value._

When you're done, move onto [Exercise 4](/exercise-4).

<BigLink href="/exercise-4" class="w-7">Exercise 4 &rarr;</BigLink>