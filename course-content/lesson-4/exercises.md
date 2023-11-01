Exercise 4: Advanced Filtering

Using data.json:

a) Use jq to filter and print only the products that have a price less than $15.
`jq '.[] | select(.price < 15)' products.json`

b) Use jq to filter and print only the products that are in stock (stock is greater than 0).
`jq '.[] | select(.stock > 0)' products.json`

c) Use jq to calculate and print the total value (price * stock) of each product.
`jq '.[] | .price * .stock' products.json`

