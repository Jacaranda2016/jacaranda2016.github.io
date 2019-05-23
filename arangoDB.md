## What is ArrangoDB?
A graph-based database


## Terms
### Collection:  a place to store your documents.
### Queries: where you write the execution codes. 
### AQL: 
#### [Tutorial](https://www.arangodb.com/docs/stable/aql/tutorial-filter.html)
  
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
   
     
  
