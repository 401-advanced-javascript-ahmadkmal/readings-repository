# class09

## Express: Router Parameters

in extended route we can put a prameter to use it leater in the code 

we can also ad prameter using middelware module 

## monogoose

Mongoose is a schema driven ORM, which gives us the opportunity to provide structure to our Mongo documents. By default, Mongo (all NoSQL Databases, really) are not structured by default. Mongoose takes some of that pain away from us as developers and allows us to provide some level of rules and validation around our data models.


### how to join two data

 populate() is a method we can use in Mongoose to connect 2 collections
Method 1: physically joining using a reference to another collection
Method 2: Virtual Population
Create a virtual field in a document pointed to a field in another one.
In pre('find') you do a collection “on the fly” which can be more efficient than storing the relation.


Pre and Post hooks (middleware)

Mongoose allows you to inject logic at various points in the lifecycle of a data record.
User can perform validation, normalization