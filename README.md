Anki Add-on for integration with Cambridge Dictionary web site - https://dictionary.cambridge.org/

IMPORTANT: This add-on doesn't use official API - only web-scraping.

What it's done (so far):
 - Creating notes from link to a word (word title, definition, gramar, IPA, sound, meanings, examples)
 - Fetching words from your wordlists - if you supply cookie for you account and wordlist IDs
 - Config settings management - save cookie, wordlist IDs
 
Please, follow these links for quick visual how-to guide.
https://ibb.co/94cq40m
https://ibb.co/WBzw37R

Your own cookie you can extract, for example, from web browser - Chrome - F12 and refresh page on cambridge 

To do (contributors are welcome):
 - OpenID authorization - through Google/Facebook
 - Native authentification - through Cambridge account
 - Token management - keeping and renewal
 - Refine UI



Added alternations by glebmark:
1) changed 5 lines in Cambridge.py: removed addition of "Meaning" of word and replaced UNDEFINED by whitespace. This "Meaning" makes learning process less efficient as it's shows on front card obvious prompt.
2) changed 6 lines in Utils.py: removed front:sound back:pronunciation template. This template isn't needed as it don't work well for English phrasal verbs such as "come along, go for, go out" and etc. Such audio files contain only first word.
