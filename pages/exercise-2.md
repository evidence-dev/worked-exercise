# Exercise 2: Using Inputs

Here we're going to use a dropdown input to filter a chart by category.

```sql categories
select category
from needful_things.orders
group by category
```

<Dropdown 
    name=category_picker
    data={categories} 
    value=category
/>

```sql category_sales_over_time
select
    date_trunc('month', order_datetime) as month,
    category,
    sum(sales) as total_sales
from needful_things.orders
group by all
order by month, total_sales
```

## a. Create a chart

_Exercise: Create a BarChart that shows the total sales for each category over time._

<Alert status=info>

**Hint:** Use a slash command to get started. See the [BarChart docs](https://docs.evidence.dev/components/bar-chart) for more info.
</Alert>

<!-- here is some space for your work -->


## b. Filter the chart using the dropdown input

_Exercise: Edit the `category_sales_over_time` query so the chart only displays data for the selected category._

<Alert status=info>

**Hint:** 

- Use the `category_picker` input in the  query as `'${inputs.category_picker.value}'`.
- See the [Dropdown docs](https://docs.evidence.dev/components/dropdown/#filtering-a-query) for more info.

</Alert>

When you're done, move onto [Exercise 3](/exercise-3). 

<BigLink href="/exercise-3">Exercise 3 &rarr;</BigLink>