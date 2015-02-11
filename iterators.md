##Descriptions of Iterators

###Instructions
Below you will find a list of methods. In the space provided below each, please provide a brief description of what this method does based upon your review of the Docs. 

###Array methods:
May be helpful to look in [Enumerable](http://ruby-doc.org/core-2.2.0/Enumerable.html) as well...

####select:
   Returns an array for all elements of an enum for which a block returns a value of true.

   If no block is given, an Enumerator is returned instead. 

####reject:
    Returns an array for all elements of an enum for which a block returns a value of fale.

    If no block is given, an Enumerator is returned instead. 

####map:
    Returns an array with the results of running block once for every elements in enum.

    If no block is given, an Enumerator is returned instead.

####detect:
    Passes each entry in enum to block. Returns the first for which block is not false, if no object matches, calls ifnone and returns its result when it is specified, or returns nil otherwise.

    If no block is given, an Enumerator is returned instead.  

####inject:
    Combines all elements of enum by applying a binay operation, specified by a block or a symbol that names a method or operator.


####partition:
    returns two arrays the first containing the elements of enum for which the block evaluates to true, thesecond containing the rest.

    If no block is given n Enumerator is returned instead.



####sort:
    Returns an array containing the items in enum sorted either according to thier own <=> method or by using the results of the supplied block. The block should return -1, 0, or +1 depending on the comparison between a and b. As of Ruby 1.8 the method Enumerable#sort_by implements a b uilt-in Scwartzian Transform, useful when key computation and comparison is expensive. 



####one:
    Passes each element of the collection to the given block. The method returns true if the block returns true exactly once. If the block is not given, one? will return only if exactly one of the collection members is true.



####none:
    Passes each element of the collection to the given block. The method returns true if the block never returns true for all elements. If the block is not given, none? wll return true only if none of the collection members is true. 



####all:
    Passes each element of the collection to the given block. The method returns true if the block never returns false or nil. If the block is not given, Ruby adds an implicit block of { |obj| obj } which will cause all? to return true when none of the collection members are false or nil.


####empty?:
    Returns true if hsh contains no key-value pairs.


####eql?:
    Returns true if hash and other are both hashes with the same content.

####include?:
    Returns true if the given key is present in hsh.

####nil?:
    Only the object nil responds true to nil?.

###Hash methods:
    Generates a Fixnum hash value for this object. This function must have the property that a.eql?(b) implies a.hash == b.hash.

    The hash value is used along with eql? by the Hash class to determine if two objects reference the same hash key. Any hash value that exceeds the capacity of a Fixnum will be truncated before being used.

    The hash value for an object may not be identical across invocations or implementations of Ruby. If you need a stable identifier across Ruby invocations and implementations you will need to generate one with a custom method.

####key?:
    Returns true if the given key is present in hsh.

####keys:
    Returns a new array populated with the keys from this hash. See also Hash#values.


####delete:
    Deletes and returns a key-value pair from hsh whose key is equal to key. If the key is not found, returns the default value. If the optional code block is given and the key is not found, pass in the key and return the result of block.

####delete_if:
    Deletes every key-value pair from hsh for which block evaluates to true.

    If no block is given, an enumerator is returned instead.
