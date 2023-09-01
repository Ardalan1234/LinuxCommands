create database:
- `use database_name`

drop database:
- `db.dropDatabase()`

create collections:
- `db.createCollectio("collection_name")`

drop a collection:
- `db.collection.drop()`

insert data into a collection:
- `db.collection.insertOne({ field: valus })`
- `de.collection.insertMany([{ field: value }, { field: value }, ...])`

retrieve documents from a specific collection:
- `db.collection.find()`

sort the documents:
- `db.collection.find().sort({ field1: 1, field2: -1 })`

restrict the number of documents returned by a query:
- `db.collection.find().limit(5)`

a query is used to specify the criteria for retrieving documents from a collection, while projection is used to specify which fields should be included or excluded:
- `db.collection.find({ query }, { projection })`
- `db.collection.find({ field1: value, fiend2: value, ... }, { field1: true, field2: false, ... })`

modify existing documents in a collection:
- `db.collection.updateOne({ filter }, { update })`
- `db.collection.update({ field1: value }, { $set: { field: value } })`
- `db.collection.update({ field1: value }, { $unset: { field: "" } })`
- `db.collectio.updateMany({ field: { $exists: {[true | false]} } }, { $set : { field: value }})`

delete documents:
- `db.collection.deleteOne({ field: value })`
- `db.collection.deleteMany({ field: value })`

comparison operators to perform comparisons between values:
 - `db.collection.find({ field: { $eq: value } })`
 - `db.collection.find({ field: { $ne: value } })`
 - `db.collection.find({ field: { $gt: value } })`
 - `db.collection.find({ field: { $gte: value } })`
 - `db.collection.find({ field: { $lt: value } })`
 - `db.collection.find({ field: { $lte: value } })`
 - `db.collection.find({ field: { $in: [value1, value2, ...] } })`
 - `db.collection.find({ field: { $nin: [value1, value2, ...] } })`

logical operators to combine multiple conditions in a query:
- `db.collection.find({ $and: [ { condition1 }, { condition2 }, ... ] })`
- `db.collection.find({ $or: [ { condition1 }, { condition2 }, ... ] })`
- `db.collection.find({ $nor: [ { condition1 }, { condition2 }, ... ] })`
- `db.collection.find({ field: { $not: { condition } } })`

an index is a data structure that improves the speed of data retrieval operations on a collection:
- `db.collection.createIndex({ field: [1 | -1] })`
