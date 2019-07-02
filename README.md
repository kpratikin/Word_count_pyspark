# Word Count in pyspark

Objective: 
To read compelete Bible.txt book and retrieve 
1. top 5 words used in the book
2. Number of unique words with 4 characters, 5 characters, 6 characters,7 characters and 8 characters.


Input file: ascii_bible.txt

Output-1: top-5 words:
Top-Word-1 <frequency-as-integer-N1>
Top-Word-2 <frequency-as-integer-N2>
Top-Word-3 <frequency-as-integer-N3>
Top-Word-4 <frequency-as-integer-N4>
Top-Word-5 <frequency-as-integer-N5>

where N1 > N2 > N3 > N4 > N5

Output-2:
<any-unique-word-with-4-characters> <frequency>
<any-unique-word-with-5-characters> <frequency>
<any-unique-word-with-6-characters> <frequency>
<any-unique-word-with-7-characters> <frequency>
<any-unique-word-with-8-characters> <frequency>
<any-unique-word-with-9-characters> <frequency>


The following additional requirements is implemented:
1. words are separated by any number of spaces or tabs
2. if any word has any special character (other than  a-z and A-Z), then that word is filtered out (dropped): with one exception: if a word ends with
       {".",  ";",  ",",  "?",  ":"} then drop that special character, and then keep/use it as a proper word.
3. Therefore a valid word can have only {a-z, A-Z}
4. all words has to be converted to lowercase
