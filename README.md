# Question #1: Turning Strings to URLs
_URLs cannot have spaces. Instead, all spaces in a string are replaced with %20. Write an algorithm that replaces all spaces in a string with %20._

_You may not use the replace() method or regular expressions to solve this problem. Solve the problem with and without recursion._

## _My Thought Process:_
* If I want to be able to find the empty spaces within an array I think I will need a loop of some kind.
* Before I can start looping through the sentence, I will more than likely need to turn it into an array using .split(), but I can’t use that for this prompt, so I will need to think of another option.
* My next thought would be to see if I am able to loop through a string without turning it into an array at all.
* On my first search, it appears that I can iterate through a string without turning it into a loop.
* While looping through the string, I may be able to use the .charAt() method which returns an index number based on the position of that character.
* I think while this is looping through, I can use a branching statement to check whether there is a space or not a space.
* I don’t need to know if there is a character in that space, I only need to know if there is a space.
* Once I have determined that there is a space, I will insert the string of “%20” in place of the space.
* On further inspection, I can also use the indexOf() method that will return the index value of a specific word or not a word.
* Once I have looped through the strings and found all spaces and replaced them with “%20”, I will return the final output in a new variable.

# Question #2: Array Deduping
_Write an algorithm that removes duplicates from an array. Do not use a function like filter() to solve this. Once you have solved the problem, demonstrate how it can be solved with filter(). Solve the problem with and without recursion._

## _My Thought Process:_
* Thankfully this input is already coming in the form of an array, so I think this will make the solution a bit easier.
* It looks like I will be receiving an array with multiple input types, such as strings and integers, but I do not know if that will affect my code process at all.
* I will more than likely need another loop for this case and it will more than likely need to be a for loop.
* I think I will need this type of loop because I want access to the index and that is a good way to get access to it while it is looping through.
* While I am looping through, I want to be able to compare the value of each index with all others.
* Once I find one with multiples of the same, I want to remove all but one and then return the altered array.
* I am not sure if I will want to alter the existing array or create a new variable with the changed array.
* My first thought for checking the value of each index is to use the sort() method, so that way all the values are sort from smallest to largest.
* I am not as interested in what the smallest, or largest items are in the array, but it will put like items next to each other by default.
* Once they are next to each other, I can loop through the array and check the value of each index with the next value coming up in the array.
* If the current index is the same as the next index value, I will remove it from the array and move on to the next index to check for the same thing.
* Once I have arrived at the end of the array, I will return a new array with all duplicate items removed.

## _How It Could Be Solved With Filter:_
* For solving this problem with the filter() method, it appears that I would not need to loop through the array, because filter() will go through the array for me.
* It looks like with filter() I can call it on the array and specify what I want to be filtering out of it and it will return the altered array.
* When calling the filter() method on the array, I want to compare the value of a word with the following word and filter it out if is the same.
* Although reading more of the documentation looks like filter will return all of the element that meets that condition and not filter them out perse.
* Because of this, I will want to check for the opposite when calling filter() because I want to return all elements that are NOT the same.
* Once it has been filtered, I will return the final array.

# Question #3: Compressing Strings
_Write an algorithm that takes a string with repeated characters and compresses them, using a number to show how many times the repeated character has been compressed. For instance, aaa would be written as 3a. Solve the problem with and without recursion._

## _My Thought Process:_
* With this problem, I will more than likely need a loop to go through every element and compare whether or not they have duplicates that are next to each other.
* While checking that value, I think I will also need a variable set to 0 that will be able to contain the number of times the letter has been repeated.
* My only concern with doing that is that how do I reset it back to 0 once I move on to the next number outside of the repeated ones.
* While reading through the prompt again as well, it looks like I only want to count the characters that are next to each other. Even if there is another character in the string that matches another, if it is not next to them, it will not be counted the same way; it will be counted as a new instance of that character.
* I am then wondering if I can use a nested loop for checking the value of a character and then counting how many times it may be repeated.
This one is racking my brain a little bit.

# Question #4: Checking for Uniqueness
_Write an algorithm that determines whether all the elements in a string are unique. You may not convert the string into an array or use array methods to solve this problem. The algorithm should return a boolean._

## _My Thought Process:_
* At this point, I know that I can use a loop for a string, but am not sure if I am going to need to do that for this problem.
* I believe there is a built-in method for strings to check for uniqueness, so I will do some research and see if that is the case.
* With my first set of research steps, it looks like I can use the includes() method to check if a string contains a certain character.
* Normally, I would need to give it a character to look for within the string, but if I use a loop, I can give it the condition of the index value to check.
* If there is a match I can then break out of the loop and return false.
* If there is never a condition that is met, I will not break out of the loop until it has gone through every character and return true if that is the case.
* At this point, I have only two possibilities that could occur: true, or false.

# Question #5: Array Sorting
_Write an algorithm that sorts an array without using the sort() method. There are many different sorting algorithms - take the time to read about the following:_
* Quick sort
* Merge sort
* Heap sort
* Insertion sort
* Bubble sort
* Selection sort
_You may implement any of the above algorithms (or your own) to solve the problem - as long as it doesn't use sort()._

## _My Thought Process:_
* Before doing any research on the above, I am already wondering if I am better off altering the existing array that is given or creating a new one with the sorted values of the first and then returning the new array.
* Looking up the definition of the Quick Sort gave me an idea to check the value of each index and push it to a new array.
* To do this I would more than likely need a nested loop the goes through each character and compares it to all other characters.
* Although, the prompt is specific on whether or not it will be an array of numbers, an array of strings, or a mix thereof.
* Because of that, I don’t think I will be able to try my initial method for sorting.
* I might be able to run a conditional statement that checks whether or not that index is an integer or a string.
* If it does turn out to be a string, I will pull the length of it and compare that value with the rest.
* With this, I will always only be comparing numerical values, which would be more consistent and easier to sort.
* The bubble sort algorithm also looks like it may be the better option in terms of sorting, but I am unclear on the syntax and why it would work.
* Because I do not understand the why of the algorithm, I do not feel confident explaining it through the process so I think I will stick to my original solution above.
* Looking at the problem one more time makes me think that it is safe to assume that I will be receiving an array of integers and do not need to error handle unless requested.
