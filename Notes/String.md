`value == value2` Here it will check the reference address.

Their is the difference between using `new` keyword and initializing a value :-

### Initializing value

Initializing a value means :-
`String s = "Something";`
`String v = "Something";`

- `s` will store in the string pool and won't create any new memory object.
- As the string `v` is same as the string `s` so v will store the same address as the `s`.
- Here we are only storing the reference.

## Using `new` Keyword

``
- Here we create the new memory address.
  
### How to compare and check the value of the string instead of the reference using `.equals()` and `.compareTo()` function

**Program of the String :- Using certain functions - `charAt()` , `length()`**

`Still to be completed later`

**How to convert the immutable string in the mutable**

- String is immutable by the nature.
- To convert the String immutable to mutable we use the String Builder and the string buffer.

# Important topics :- String Array & String Array List


### Finding the substring in the array using `substring()` function


### Trim and split function

**Using trim**

	s = "___Hello___gla___"; // here taking the white spaces 
	s.trim(); // This is always remove the starting and the ending white spaces.

**Using split**

	s = "I_Love_gla"; // containing spaces.
	s.split() // convert the string the array on the basis of the spaces.

#### Code to remove all the spaces 

	String original = "He llo Wo r l d";
	String noSpaces = original.replaceAll("\\s+", "");
	System.out.println(noSpaces);  // Output: HelloWorld

#### Code to remove everything except something that we wanted

|Symbol|Meaning|
|---|---|
|`[]`|A **character class** — matches any **one character** inside the brackets|
|`a-z`|Lowercase letters from a to z|
|`A-Z`|Uppercase letters from A to Z|
|`0-9`|Digits from 0 to 9|
|`^` (inside `[]`, at the **start**)|**Negation** — means “anything **not** listed here”|

	String s = "Hello, World 123!";
	String cleaned = s.replaceAll("[^a-zA-Z0-9]", "");
	System.out.println(cleaned);  // Output: HelloWorld123


