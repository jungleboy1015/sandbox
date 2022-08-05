### Day 3: August 5, 2022
**Today's Study**: Udemy course section 4 on conditional logic.

**Notes:** 
* Legit = (set it) vs. == (don't forget it).

### Day 2: August 4, 2022
**Today's Study**: Finished Udemy course section 3 on functions through debugging assignment; read stack overflow on signed vs. unsigned integers.

**Notes:** 
* Signed vs. unsigned integers - Unsigned: consists of only non-negative values i.e 0 to 255.  Signed: It consist of both negative and positive values but in different formats like 0 to +127 OR -1 to -128
* local variables will supercede state variables - Remix will throw an error saying 'shadowed' if you declare a local with same name as a state variable.

### Day 1: August 3, 2022
**Today's Study**: Udemy course part 3, first 5 videos; reviewed https://secureum.substack.com/p/solidity-101 for things I don't yet understand (lots); 

**Notes:** bytes vs. strings:  bytes for arbitrary-length raw byte data and string for arbitrary-length string (UTF-8) data. bytes1 to bytes32 are much cheaper.

**Today's Project:** Decaying yearly membership.  Looked at https://ethereum.stackexchange.com/questions/57918/how-can-i-convert-between-a-solidity-timestamp-and-year-month-day-hourminutese?rq=1 and https://github.com/bokkypoobah/BokkyPooBahsDateTimeLibrary to start to think about how decaying ragequittable membership might work based on time.  Is the cheap / easy solution just store the timestamp at minting, and use the formula:  

((timestamp at ragequit - timestamp at minting) / 31536000 (seconds in 365-day year)) * original purchase price
