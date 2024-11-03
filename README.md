I started this week's project by relying on the previous contract, that is simpleStorage.sol. In creating a "storage" storage location for my contract, I relied on the first code that I created at 
the beginning of the contract. Which is "uint256 public favouriteNumber;", and it is state variable in nature. And evey state variable has a storage location of Storage. Simlarly, in creating the 
"memory" storage loaction, I created the function whatName() to store temporary stores the name of the user in string form. And in a similar fashion, I created the concatenateString() function 
to temporary concatenate the string that the user will input to the string " is awesome!" which is not mutable. And the "calldata" storage location is used to do that. And this
"string memory newString = string(abi.encodePacked(_inputString, " is awesome!"));" line of code was used to do the concatenation.



And in implementing the mapping, "mapping(string=>uint256) public nameToFavouriteNumber;" this code was written to declare it by assigning the name of the user to his favouriteNumber.
Which was implemented using the addPerson() function, where this "nameToFavouriteNumber[_name] = _favouriteNumber;" code was used to implement the mapping by using the function parameters.


And finally, In implementing the event and emit variable. Thsi code "event numberUpdated(uint256 newNumber);" was written to declare an event named numberUpdated, and this allows to be accessed
by external contracts or applications. And in the storeNumber() function, this code "emit numberUpdated(_favouriteNumber);" was written to log the event. Which indicates that, any number input 
by the user will be updated by the blockchain.
