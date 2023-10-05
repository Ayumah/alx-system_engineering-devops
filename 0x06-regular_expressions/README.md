0x06. Regular expression

Background Context
For this project, you have to build your regular expression using Oniguruma,
a regular expression library that which is used by Ruby by default.
Note that other regular expression libraries sometimes have different properties.

Because the focus of this exercise is to play with regular expressions (regex),
here is the Ruby code that you should use, just replace the regexp part, meaning the code in between the //:

example.rb
	#!/usr/bin/env ruby

	puts ARGV[0].scan(/127.0.0.[0-9]/).join

	./example.rb 127.0.0.2

	127.0.0.2

	./example.rb 127.0.0.1

	127.0.0.1

	./example.rb 127.0.0.a


Tasks
0. File: 0-simply_match_school.rb - The regular expression must match School

1. File: 1-repetition_token_0.rb - Find the regular expression that will match the below cases
	hnb
	hbtn
	hbttn
	hbtttn
	hbttttn
	hbtttttn
	hbttttttn

2. File: 2-repetition_token_1.rb - Find the regular expression that will match the below cases
	htn
	hbtn
	hbbtn
	hbbbtn

3. File: 3-repetition_token_2.rb -  Find the regular expression that will match the below cases
        hnb
        hbtn
        hbttn
        hbtttn
        hbttttn

4. File: 4-repetition_token_3.rb -  Find the regular expression that will match the below cases
        hnb
	hban
        hbtn
        hbttn
        hbtttn
        hbttttn

5. File: 5-beginning_and_end.rb - The regular expression must be exactly matching a string that starts with h ends with n and can have any single character in between

6. File: 6-phone_number.rb - This task is brought to you by a professional advisor Neha Jain, Senior Software Engineer at LinkedIn.

Requirement: The regular expression must match a 10 digit phone number.

7. File: 7-OMG_WHY_ARE_YOU_SHOUTING.rb - The regular expression must be only matching: capital letters

8. File: 100-textme.rb - Your script should output: [SENDER],[RECEIVER],[FLAGS]
	The sender phone number or name (including country code if present)
	The receiver phone number or name (including country code if present)
	The flags that were used 
