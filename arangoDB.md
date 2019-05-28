## What is ArrangoDB?
A graph-based database


## Terms
### Collection:  a place to store your documents.
### Queries: where you write the execution codes. 
### AQL: 
#### [Tutorial](https://www.arangodb.com/docs/stable/aql/tutorial-filter.html)
Retrieving data from the database with AQL does always include a RETURN operation.

#### High-level Operations

>The following high-level operations are described here after:
- FOR: Iterate over all elements of an array.
- RETURN: Produce the result of a query.
- FILTER: Restrict the results to elements that match arbitrary logical conditions.
- SORT: Force a sort of the array of already produced intermediate results.
- LIMIT: Reduce the number of elements in the result to at most the specified number, optionally skip elements (pagination).
- LET: Assign an arbitrary value to a variable.
- COLLECT: Group an array by one or multiple group criteria. Can also count and aggregate.
- REMOVE: Remove documents from a collection.
- UPDATE: Partially update documents in a collection.
- REPLACE: Completely replace documents in a collection.
- INSERT: Insert new documents into a collection.
- UPSERT: Update/replace an existing document, or create it in the case it does not exist.
- WITH: Specify collections used in a query (at query begin only).
  
  * INSERT document INTO collectionName. document----->key-value pairs.
  
   > Each document needs a unique _key, which identifies it within a collection. 
   >The _id is a computed property, a concatenation of the collection name, a forward slash / and the document key. 
   >It uniquely identies a document within a database. _rev is a revision ID managed by the system.
   >Document keys can be provided by the user upon document creation, or a unique value is assigned automatically. 
   >It can not be changed later. All three system attributes starting with an underscore _ are read-only.
   
  * LET variableName = valueExpression
  * FOR variableName in expression is used to iterate over each element of the data array.
  * ```
     FOR c in Characters
        RETURN c
    ```
  * Query a specific document
    ``` TURN DOCUMENT(document_id) ```
     or
     ``` RETURN DOCUMENT(collection_name, document_key) ```
     
   * Query multiple documents
      put all the documents in a list
##### AQL Functions
AQL supports functions to allow more complex computations and function name is case-insensitive. 
Syntax for AQL functions:
```FUNCTIONANME(arguments)```

### How to install and run a local ArangoDB server?

### How to use the web interface to interact with it?

### How to store data in the database?

### How to query the database to retrieve the data again?

### How to edit and remove existing data?



      
   * Update a document
    ``` UPDATE document_key WITH {key_name:new_value} IN Characters ```
    if the key does not exist, a new key-value pair would be inserted into this document.
    
   * Replace the entire document
   
   ``` 
   REPLACE document_key WITH {
       key_1: value_1,
       key_2: value_2,
       key_3: value_3
   } IN Characters 
   ```
   
   * Delete document
   ``` REMOVE dOcument_key IN collection_name ```
   
   * Filters
   
     
  
