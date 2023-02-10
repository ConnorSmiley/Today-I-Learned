# Show all database

-`show dbs`

# switch databases

-`use <database name> `

# Show the collection in a database 

-`show collections `

# create a new database

-`use newDB `
-`show dbs `

# show current database

-`db `

# Create collection

-`db.<create collection>('something') `

# insert a document

-`db.<db name>.insert({
id:0,
company: "name",
products : ['coffee', 'sugar'],
contacts : {
    name: 'Jim',
}}) `

# Query data 

-`db.<name>.find() `

# delete document

-`db.<name>.remove{(id:0)} `

# to insert multiple documents 

-`db.<name>.insertMany([
{ id : 0,
company: "lasosta",
address : "23 lost street-NY",
overdue_invoices : 20,
products: ['sugar', 'coffee'],
creation_date : Date(),}, { id : 1, company: "vanilla factory", address : "23 great street-CA", overdue_invoices : 21, products: ['milk', 'vanilla'], creation_date : Date(), },{ id : 2, company: "john & sons", address : "23 found street-TX", overdue_invoices : 22, products: ['books', 'magazines'] }])`
  `

# Choose a document based on criteria
-`db.<name>.find({<whatever>:<whatever>}) `

# Counting 
-`db.<name>.find({<whatever>:<whatever>.count()})`

# Count (asending, descending)
-`db.<name>.find().sort({<whatever>:<whatever>}) `

# UpDate Safely
-`db.<name>.update({<whatever>:<whatever>}, 
{$set: {<whatever>:<whatever>}
})
db.<name>.find()
`


# Incrementing 
-`db.<name>.update({<whatever>:<whatever>}, {$inc: {<whatever>:<whatever>}}) 
db.<name>.find()
`

# Rename
-`db.<name>.update({<whatever>:<whatever>}, {$rename: {<whatever>:<whatever>}
}) 
db.<name>.find()`

# update array in id 0
-`db.<name>.update({<whatever>:<whatever>}, {$set: {<whatever>:<whatever>}}) `
db.<name>.find()

# 
-` `

