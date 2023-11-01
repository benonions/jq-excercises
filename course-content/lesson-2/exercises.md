Exercise 2: Filtering and Mapping

Given the same JSON data 'pets.json' as in Exercise 1, use jq to perform the following operations:

a) Filter and print only the pets that are of species "Dog".
`jq '.pets[] | select(.species == "Dog")' pets.json`


b) Map and print only the names of the pets.
`jq '.pets[] | .name' pets.json`

