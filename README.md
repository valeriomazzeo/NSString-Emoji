# NSString+Emoji
[![Pod Version](http://img.shields.io/cocoapods/v/NSString+Emoji.svg?style=flat)]()
[![Pod Platform](http://img.shields.io/cocoapods/p/NSString+Emoji.svg?style=flat)]()
[![Pod License](http://img.shields.io/cocoapods/l/NSString+Emoji.svg?style=flat)](http://opensource.org/licenses/MIT)

## GETTING STARTED

NSString (Emoji) extends the NSString class to provide custom functionality
related to the Emoji emoticons.

Through this category, it is possible to turn cheat codes from 
[Emoji Cheat Sheet](http://www.emoji-cheat-sheet.com) into unicode emoji characters
and vice versa (useful if you need to POST a message typed by the user to a remote service).

## USAGE

There are just two methods, which should be very self explanatory:

	/**
	 Returns a NSString in which any occurrences that match the cheat codes
	 from Emoji Cheat Sheet <http://www.emoji-cheat-sheet.com> are replaced by the
	 corresponding unicode characters.
 
	 Example: 
	 "This is a smiley face :smiley:"
 
	 Will be replaced with:
	 "This is a smiley face \U0001F604"
	 */
	- (NSString *)stringByReplacingEmojiCheatCodesWithUnicode;

	/**
	 Returns a NSString in which any occurrences that match the unicode characters
	 of the emoji emoticons are replaced by the corresponding cheat codes from
	 Emoji Cheat Sheet <http://www.emoji-cheat-sheet.com>.
 
	 Example:
	 "This is a smiley face \U0001F604"
 
	 Will be replaced with:
	 "This is a smiley face :smiley:"
	 */
	- (NSString *)stringByReplacingEmojiUnicodeWithCheatCodes;

## LICENSE

NSString+Emoji is available under the MIT License (MIT).

Copyright (c) 2013 Valerio Mazzeo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## AUTHOR

[Valerio Mazzeo](https://twitter.com/valeriomazzeo)