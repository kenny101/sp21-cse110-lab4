# part a:
1. values added:  20
2. final result:  20
3. values added:  20
4. 13 is an error because declaring with let only declares the variable locally in the braces. Outside braces, result is destroyed
5. line 9 doesn't get executed because at line 7, we tried to change result but the compiler gave us an error because we tried to change a const variable
6. line 13 doesn't get executed because at line 7, we tried to change result but the compiler gave us an error because we tried to change a const variable
# part b:
1. line 12 prints 3 because there are 3 items in prices and the variable 'i' is a global variable
2. line 13 prints 150 because it saved the last item stored in discountedPrices was 300 * (1 - 0.5) which is equal to 150
3. line 14 also prints 150 because finalprice was Math.round(150 * 100)/100; which is also 150
4. the function will return the new array discounted which is [ 50, 100, 150 ] because the function read each input array and reduced it by 0.5 which was our discount input and pushed it into our new array for each input which turned out to be [ 50, 100, 150 ]
5. line 12 is a ReferenceError because i was not defined outside the for loop since we defined it with the '
let keyword
6. line 13 is a ReferenceError because discountedPrice was not defined outside the for loop since we defined it with the '
let keyword
7. line 14 returned 150 because finalPrice was declared in the same scope as line 14 and Math.round(150 * 100)/100 returns 150
8. line 15 returned [ 50, 100, 150 ] because discounted was declared in the same scope that we returned it
9. line 11 gives us a compiler error because outside the scope of the for-loop, i is destroyed so it is not defined after that
10. line 12 returned 3 because that was the length prices that we pushed in our for loop. length is in the same scope as line 12 so there would be no undefined variables for length
11. it returned [ 50, 100, 150 ] because that was what we pushed into the array. there were no problems with this because discountedPrice was not changed (i.e. set equal to something else) but redeclared.
12a. student.name
12b. student["Grad Year"]
12c. student.greeting();
12d. console.log(student["Favorite Teacher"].name);
12e. console.log(student.courseLoad[0]);
13a. Output was '32' because 2 was turned into a string and 3 concatinated with 2. 
13b. Output was 1 because the string 3 was converted to a number and 3-2=1
13c. Output was 3 because null was converted to 0 and 3+0=3
13d. Output was '3null' because null was converted to a string and then concatenated with the string 3 
13e. Output was 4 because true was converted to the number 1 and added to 3 which is 4
13f. Output was 0 because both false and null are 0 when added and 0+0=0
13g. Output was '3undefined' because '3' was concatinated which undefined and undefined was casted into a string
13h. Output was NaN because undefined is NaN so performing '3' - undefined is impossible thus returned NaN
14a. Output was true because '2' casted into the number 2 and 2 > 1 is true
14b. Output was false because we first compare the number 2 and 1 in the respective strings '2' and '12' and 2 < 1 is false
14c. Output was true because the string '2' was converted to number 2 and 2==2 is true.
14d. Output was false because === treats numbers and strings differently
14e. Output was false because true is the number 1 and 1 == 2 is false.
14f. output was true because boolean(2) is nonzero thus returns true.
15. == does not have strict typing checks while === has strict typing checks. (i.e. === checks that for example numbers are not strings)
17. The result is [ 2, 4, 6 ]. for every number in the array, the callback function doSomething multiplies the value by 2 which is why our output array is twice the value that we inputted.
19. The output was 1 \n 4 \n 3 \n 2. (where \n is a newline character). This was because 1 was printed first, 2 was awaited for a second, 3 was waited for 0ms but not printed yet. 4 was not awaited so it is printed after 1. 3 is printed after 4 because it had a much shorter await time than 2. 2 is last because it was awaited the longest.