### Day 8: August 14, 2022
**Today's Study**: Udemy vids 58-59 'for loops'

### Day 7: August 11, 2022
**Today's Study**: Udemy vids 55-57 on operators.  Just one note:  mod 0 causes a failed assert and uses all available gas - big problem.

### Day 6: August 10, 2022
**Today's Study**: Udemy vids 48-54 on comparison and logical operators.

**Notes:**
* Logical operators - && (and) || (or) ! (not)
* Assignment operators - += is short hand for x + x + y

### Day 5: August 8, 2022
**Today's Study**: Udemy vids 36-47 on conditional logic, scope and arithmetic operators.

**Notes:**
* solidity can't return fractions - "5 / 7" will equal 0
* After this course, plan to spin through cryptozombies again.

### Day 4: August 7, 2022
**Today's Study**: Udemy vids 34-35 on conditional logic.

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
