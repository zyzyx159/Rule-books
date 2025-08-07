- [x] Core Rule book
	- [x] Split the book into files by chapters
- [ ] Galaxy of Guns
	- [ ] Need to do the links
		- [ ] Done up to Ammunition
- [ ] Inquisitor's Handbook
	- [x] Splitting the book into files by chapters
	- [x] Split out alternative paths
- [x] Poisons and Toxins
- [x] Tools of the Trade


Find Replace Script for Chem Links

You can achieve this using a regular expression in a text editor or script that supports regex, such as IntelliJ IDEA or a Python script. The pattern `$$#Chem-Use$$` will match the literal text `[[#Chem-Use]]`, and the replacement `$$[Chem-Use](Skills.md#Chem-Use)$$` will generate the desired link format. The `Chem-Use` part within the brackets and the anchor will be dynamically replaced based on the actual text found within the `#` and `]]` delimiters.

For example, in a tool like IntelliJ IDEA, you would use the "Find in Files" and "Replace in Path" functionality with a regular expression. The search pattern would be `$$\[\[#(.*?)\]\]$$` and the replacement would be `$$[$1](Skills.md#$1)$$`, where `$1` captures the text between `#` and `]]`. This approach allows the script to handle different `Chem-Use` values dynamically.