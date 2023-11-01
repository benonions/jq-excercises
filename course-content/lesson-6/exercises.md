Exercise 6: Advanced Mapping

Given the following JSON data in a file named grades.json:

a) Use jq to calculate and print the average grade for each student.
`jq '(.students[] | .grades | add) / (.students[].grades | length)' grades.json`

b) Find and print the student with the highest average grade.
`jq 'max_by(.grades | add / length) | .name' grades.json`

