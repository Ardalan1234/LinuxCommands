Select Database:
- `SELECT index`

To Set a key-value pair:
- `SET key value`

To Get a key-value pair:
- `GET key`

To Delete a key-value pair:
- `DEL key`

To Set multiple key-value pairs:
- `MSET key1 value1 key2 value2 ...`

To Get multiple key-value pairs:
- `MGET key1 key2 ...`

To Get a range of characters:
- `GETRANGE key start end`

To Set a substring of the value of a key:
- `SETRANGE key offset value`

To increment the integer value:
- `INCR key`

To decrement the integer value:
- `DECR key`

To increment and decrement the integer value by a specified amount:
- `INCRBY key increment`
- `DECRBY key decrement`

To perform both operations in a single command and get the value as a result:
- `SET key value GET`

To add one or more members to a set:
- `SADD key member [member ...]`

To remove one or more members from a set:
- `SREM key member [member ...]`

To perform a union operation on multiple sets:
- `SUNION key [key ...]`

To check if a member exists in a set:
- `SISMEMBER key member`

To retrieve all members from a set:
- `SMEMBERS key`

To insert one or more values at the beginning (left side) of a list:
- `LPUSh key element [element ...]`

To insert one or more values at the end (right side) of a list:
- `RPUSH key element [element ...]`

To retrieve elements from a list:
- `LRANGE key start stop`

To remove and return the first element (leftmost element) of a list:
- `LPOP key [count]`

To remove and return the last element (rightmost element) of a list:
- `RPOP key [count]`

To get the length (number of elements) of a list:
- `LLEN`

To retrieve the element at a specific index in a list:
- `LINDEX key index`

To get the position of an element within a list:
- `LPOS key element [RANK rank]`

To set individual field-value pairs:
- `HSET key field value [field value ...]`

To retrieve the value of a specific field:
- `HGET key value`

To retrieve all field-value pairs in a hash:
- `HGETALL key`

To delete a field (and its associated value) from a hash:
- `HDEL key field [field ...]`

To retrieve all the field names (keys) of a hash:
- `HKEYS key`

To retrieve all the values of a hash:
- `HVALS key`
