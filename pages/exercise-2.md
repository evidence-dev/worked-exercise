# Exercise 2

Here we're going to use some of the more powerful Evidence features.

## 1. Write a query to get category sales

Exercise: Write a query to return the category name and the total sales for that category.

<!-- here is some space for your work -->

## 2. Create an `{#each}` loop 

Exercise: Write a [loop](https://docs.evidence.dev/core-concepts/loops) that displays the category name and the total sales for that category in a list.


<Alert status=info>

**Hint:** The syntax for loops is

```html
{#each query_name as row_alias}
    
Some content and data from rows {row_alias.column_name} 

{/each}
```
</Alert>

<!-- here is some space for your work -->


## 3. Add an `{#if}` condition to the loop

Exercise: Add an [if statement](https://docs.evidence.dev/core-concepts/if-else) inside the loop so that it only displays categories with sales greater than a particular value.