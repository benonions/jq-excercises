Exercise 3: Nested JSON

Using nested.json:

a) Use jq to extract and print the person's name.
`jq '.person.name' nested.json`

b) Use jq to extract and print the city from the address.
`jq '.person.address.city' nested.json`

c) Use jq to print all the hobbies of the person.
`jq '.person.hobbies[]' nested.json`
