# FirstUpper

### Summary
This is a basic plugin for Notepad++ that gives the user different tools for capitalization.

### Features
##### Capitalize the First Letter of Specific Words in a Selection
Select some text and press ```Ctrl+Alt+U``` to capitalize the first letter of the words in the selection. This is meant for proper capitalization of titles based on the Chicago Manual of Style and specific words will not be capitalized. The plugin uses the text file "FirstUpperForbiddenWords.txt" as the list of words that should not be capitalized.

##### Capitalize the First Letter of the First Word of All Sentences in the Document
This does not have a keyboard shortcut and must be accessed from the Plugins menu. This feature will look for typical punctuation that you use to end a sentence such as periods or question marks and it will capitalize the first letter of the first word directly after that punctuation. Currently this feature does not understand that file names should be excluded.

##### Find and Capitalize All Titles in a Markdown File
The option "Capitalize All Markdown Titles" will find and properly capitalize all of the markdown titles in the document. It supports Setext style ("=" or "-") headings and Atx style (one or more "#") headings.

##### <span style="color:red;">[NEW]</span> Camel Case Last Word Typed
Use ```Alt+Shift+U``` to convert the last typed "variable" to camel case. This feature uses a dictionary of words to find "real" English words and when it finds a word it will capitalize the word. The feature does not care if the word has any kind of upper or lower case characters already.  
For example the variables

    var thisawesomevariable;
    var HELLOTHERE;
	var hOWarEYoU;

become

    var thisAwesomeVariable;
	var helloThere;
	var howAreYou;

### How to Use
##### Installation
To install this plugin download the files from the folder labeled "PluginInstallFiles". Place each file in the directories as follows    
<ul>
	<li>"FirstUpper.dll" goes in the "Notepad++/plugins" directory.</li>
	<li>"FirstUpperForbiddenWords.txt" and "FirstUpperDAWG.bin" go in the folder "plugins/doc/FirstUpper". You must create this folder.</li>
	<li>"DawgSharp.dll" goes in your "Notepad++" root directory with the notepad executable.</li>
</ul>
I apologize for the difficult install procedure. I will improve this soon.

##### Usage
Select an option from the plugins menu under "FirstUpper".  
For the option "Capitalize Selected Title" you can use the shortcut ```Ctrl+Alt+U```.  
For the option "Camel Case Last Word Typed" you can use the shortcut ```Alt+Shift+U```.

##### Forbidden Word List
If there are words you wish to add to the list of "forbidden" words so as to cause the plugin to not capitalize them, simply add the word(s) to the "FirstUpperForbiddenWords.txt" file. **Make sure each word is on its own line.** If there are specific words in the "forbidden" list you wish to capitalize, you must open the text file and you may either delete the line that contains the word or place an asterisk (```*```) in front of the word. 

### Planned Features
Although this is a very simple and largely useless plugin, I enjoy playing with it and therefore I will continue adding features as I have time.

##### Settings Menu
I wish to implement a simple settings window of some kind. Perhaps instead of using a text file for the forbidden words, I will use the settings window to allow the user to edit the forbidden words within Notepad++. This settings window will also allow you the option to capitalize the first letter of *all* words. I would also like to implement support for capitalizing initials so that "j.f.k" becomes "J.F.K". Many of these features can be in the plugins menu such that the user may simply select the desired command in the menu.

zkirkland
