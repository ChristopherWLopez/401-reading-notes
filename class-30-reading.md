# class 30 reading

hash- a hash is the return of an algorithm that takes in a string and converts it into a value that can be used for security (or another purpose). If its a hash table than it is used tp determine the index of an array

buckets - a bucket is whats contained in each index of the array of each hashtable. Each index is a bucket, each bucket can contain multiple key/ value pairs if a collision occurs.

collision - when one more than one key gets hashed to the same location.

## when do we use them ?

- when we want to hold unique values
- Dictionary
- Library

## what are they ?
HT's are a data structure that uses key value pairs. This is like a `node` or a `bucket` has both a key and a value

we are able to store the key into the ds and quickely retrieve the value. We do this using `hash` (ability to encode) `hashing` will eventualy get mapped to a specific location in the data structure.

instead of having to loop throuh an array of data, we are able (0(n) because we are having to search through every piece of data to find the peice. we want).

an array is actually pretty easy to find data because we can use the index, 0(1) our hash map uses that readtime by hash function to place that certain item into a specific location which we could easily find by its address. 

input: key
output: integer

output determined by their input.
no randomness. pure function.

we use the int. to determine where the key/value is to be placed in array. 

takes the key, run through hash code to get a number use number to index array.

``Add or multiply all the ASCII values together.
Multiply it by a prime number such as 599.
Use modulo to get the remainder of the result, when divided by the total size of the array.
Insert into the array at that index.``

each bucket starts as null. 

collision happens when one or more keys go to the same bucket. 

if two keys to same index then we call `.Add(key, val)` if there is a collision we can initialize a linked list in each bucket.

To store:
take key,
calculate hash of key,
use mod to convert hash to index
store key with value

to read: 
accept key,
calculate hash of key,
use mod to convert the has into an array index,
use array I to access the linked lis (bucket)
search bucket looking forthe node with the key and value pair.

can computed load factor, this tells us how full the ht is you can calculate and add more buckets.

set()
get()
has()
keys()
hash()