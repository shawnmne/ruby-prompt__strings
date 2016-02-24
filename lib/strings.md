---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

Strings are a sequence of characters denoted by single or double quotes.

# What are some examples of information that would be Strings as opposed to some other data type?

name = "Shawn Michaud"
address = "4245 South St."
wife_name = "married to Melissa"

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

name = "Ada Lovelace"
puts name[5]
puts name[7]

When trying to retrieve a character that doesn't exist it will return nil


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes. The negative symbol means to start from the last characater and count backwards. -1 is the very last characater so -6 would be the the sixth from the end of the string
name = "melissa"
name[-6] = "e"

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

The string operator .sub will replace a first occurence of a string to be replaced .gsub will do it globally.
puts "Sumeet Jain".sub("ee", "!!") would work but also 
puts "Sumeet Jain".gsub("e", "!") would also work
