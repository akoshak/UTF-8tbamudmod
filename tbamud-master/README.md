Files for tbaMUD.

This is a modification of tbaMUD 3.67, based on circleMUD, to allow for creating MUDs with non-Latin characters. It deals with UTF-8 characters by converting between ASCII and UTF-8 one line at a time for input and output, where the characters remain in ASCII within the system.

The translation files are in lib/translation/. There is 3 files there, English to another language for when the system creates a message, other to English to translate input from the user for the system, which remains in English, and the other file with "everything else." In lib/translation/english_to_others , you have the English phrase on one line and the other language translation (here Arabic version) on the other line, alternating. As you run the program and you see new strings you've never translated, they will get dumped to lib/translation/untranslated automatically. In C to print a string and a number, you have to use format strings, like "The player deals %d points of damage" If you keep the %d, the numbers can change to anything while translating only once. 

