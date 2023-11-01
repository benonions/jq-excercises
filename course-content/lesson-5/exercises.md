Exercise 5: JSON Manipulation

Given the following JSON data in a file named data.json:

a) Use jq to add a new person with the name "David" and age 30 to the "people" array. Print the modified JSON.
`jq '.people += [{"name": "David", "age": 30}]' data.json`

b) Use jq to sort the "people" array by age in ascending order. Print the sorted JSON.
`jq '.people |= sort_by(.age)' data.json`

