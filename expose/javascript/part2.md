1. '3'. The last value of i before the loop exited will be printed to the console. Namely, as the for loop exits when i == prices.length and prices has 3 entries, line 12 would log '3' to console. This is because the iterator i was declared as a var and thus has function scope.
2. '150'. The last value of discountedPrice in the for loop would be printed to the console, namely 150. This is because discountedPrice was declared with var and thus has function scope. Then, because the loop was run at least once, the variable still exists after the loop exits.
3. '150'. The last value of finalPrice in the for loop would be printed to console, namely 150. finalPrice was declared outside the loop, but is changed every time the loop is run. Therefore, its value at the end of the loop is simply the value during the most recent iteration.
4. This function returns an array of length 3 with entries [50, 100, 150] corresponding to a 50% discount on the prices in the input array. Each price in the prices array is multiplied by 0.5 and then rounded before being added to the return array. Because none of the input values are decimals, rounding does nothing and the result is just 50% of all the inputs in prices.
5. This code will throw a ReferenceError, as let i had block scope and those longer exists at line 12.
6. This code will throw a ReferenceError as let discountedPrice had block scope inside the for loop and thus no longer exists at line 13. 
7. '150' will be printed to the console. let finalPrice has block scope, but the block is the function and therefore it is a valid reference at line 14. More so, its value was changed in the for loop and is just the most recent value held before the loop exited.
8. Like before, this function an array of length 3 with entries [50, 100, 150] corresponding to a 50% discount on the prices in the input array. Because all the variales were used in their correct scope, the answer doesn't change from before.
9. This code will throw a ReferenceError, as let had block scope and thus no longer exists at line 11.
10. '3' will be printed to the console as const length was set to the length of prices (3) on line 4 and line 12 is still in block scope of that.
11. This function will return [50, 100, 150]. All the variables in their correct scopes, so there isn't an error. Thus, the result is just the discount (50%) applied to each price.
12. 
	a. student.name
	b. student['Grad Year']
	c. student.greeting()
	d. student['Favorite Teacher'].name
	e. student.courseLoad[0]
13. 
	a. '32', because ints get converted to their string representation under addition
	b. 1, because subtraction causes strings to get converted to ints
	c. 3, because null converts to 0 when parsed as an int
	d. '3null', because null converts to 'null' with a string
	e. 4, because true converts to 1 when parsed as an int
	f. 0, because both null and false become 0s as numbers
	g. '3undefined', because undefined becomes itself as a string when concatenated
	h. NaN, because undefined is NaN under numeric conversion rules
14.
	a. true, because '2' is converted to the number 2 and 2 > 1
	b. false, compared as strings '2' is greater than '12' because '2' is a bigger character than '1'
	c. true, '2' is converted to a string and thus 2 == 2
	d. false, they are not the same type
	e. false, true is converted to 1 and 1 =/= 2
	f. true, 2 is converted to true b/c it is nonzero and true === true
15. == compares if two variables are converted to the same value, but === compares if two variables _are_ the same value
16. part2-question16.js
17. The result is [2, 4, 6]. Each element in the input array is passed to the doSomething() function passed into the function as the callback parameter. This function multiplies by 2. Thus, the result is all the original numbers multiplied by 2.
18. part2-question18.js
19. This code prints 1,4,3,2. Obviously 2 comes last as it is on a 1 second delay. 3 comes after 4 because the 0 millisecond delay forces the code to run when ready, not instantly.