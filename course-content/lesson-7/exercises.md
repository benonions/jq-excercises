Exercise 7: Conditional Filtering

Given the following JSON data in a file named weather.json:

a) Use jq to filter and print only the days when it's raining.
`jq '.forecast[] | select(.rain == true) | .day' weather.json`

b) Use jq to filter and print the days with a temperature above 80 degrees.
`jq '.forecast[] | select(.temperature > 80) | .day' weather.json`
