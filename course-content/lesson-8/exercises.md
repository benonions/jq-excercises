Exercise 8: String Manipulation

Given the following JSON data in a file named books.json:

a) Use jq to concatenate the "title" and "author" fields for each book into a single string, separated by a hyphen (-). Print the modified JSON.
`jq '.books[] | .title + " - " + .author' books.json`

b) Use jq to find and print the titles of books authored by "George Orwell."
`jq '.books[] | select(.author == "George Orwell") | .title' books.json`

