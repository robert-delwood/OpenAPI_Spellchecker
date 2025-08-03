# OpenAPI_Spellchecker
A spellchecking tool and a word analyzer for OpenAPI files.

## Introduction
*OpenAPI_Spellchecker* is a word analyzer.
It seperates all the contents of an OpenAPI into individual words.
The word list can be further refined by removing words that are all numbers, have numbers in them, and camel cased words.
Camel cased words are those with capital letters in a position other than the first letter.
Those are typically field or variable names.
What's left are sorted and have duplicates removed.
Misspelled words are identifed.
That list is also automatically copied to the clipboard for pasting into other documents as wanted.

## Prerequisites
* *OpenAPI_Spellchecker* runs under Windows only.
The plans for a Mac version are uncertain.
* The OpenAPI file must be less than version 3.1.0. If this is a problem, in many cases, the OpenAPI files's version number can be changed to 3.0.3 safely.
* The OpenAPI file must be well-formed and conform to the OpenAPI specification.
* Files can be either JSON or YAML.
* For best results I recommend using a fully deferenced OpenAPI file.
That is, a file with no $ref statements.
In most cases $ref statements are accurately handled but due to OpenAPI coding differences, I can't assure accurate reporting.

## Downloading *OpenAPI_Spellchecker*
To download *OpenAPI_Spellchecker*,
1. Navigate to: **https://download-directory.github.io**
2. Paste this URL into the text box: **https://github.com/robert-delwood/OpenAPI_Spellchecker/tree/main/OpenAPI_Spellchecker/OpenAPI_Spellchecker_Project**
3. Click Enter. This displays a save file dialog.
1. Navigate to the download location of your choice.
2. You muight want to change the download name to something like **OpenAPI_Spellchecker.zip**.
   This download application makes up it's own names.
1. Select **Save**. This saves the file to that location.
1. Double click **OpenAPI_Spellchecker.zip**, or whatever you just named it.
   This will unzip the file to the selected location.
   This will create a folder at the location named **OpenAPI_Spellchecker**.
   The extracted contents will be loaded into that folder.
   There are no other dependencies.

## Running OpenAPI_Spellchecker
To run *OpenAPI_Spellchecker*,
1. Double click the application OpenAPI_Spellchecker.exe.
It opens to the *OpenAPI_Spellchecker* window.
By default, it is set to Show misspellings.
1. Select **Open OpenAPI file**. This shows the file open dialog.
   Navigate to, and then select, the target OpenAPI file.
   It may either JSON or YAML.
   Processing should be automatic.
1. Select **Process file** should it not process automatically when an OpenAPI file is first selected
   It may also be selected to force processing an additional time, if needed.

The View criterion may be changed.
If so, select Process file again.

Processed word lists are automatically copied to the clipboard.
Individual words may be copied to the clipboard by either double clicking the word, or selecting **Copy selected word clipboard**.
Without any additional involvement with the application, you can paste the clipboard into another document.
For example, this may be in Microsoft Word or as any text file.

## View criterion
The following options are available.
In each case, the list removes duplications and is sorted in ascending alphabetic order.

**Show misspellings**. This shows only the misspellings.
This is the default selection.<br>
**Show all words**. This shows all the words.<br>
**Show words with midfix numbers**. This shows only words that have the letters and numbers.<br>
**Show words with numbers only**. This shows words that are only numbers.<br>
**Show words with upper- and lower-case letters**. This show words that have both upper- and lower-case letters other than as the first character.
This typically includes field names. It excludes words that are only uppercase.<br>
**Show words with uppercase only**. This shows words that are only uppercase. Typically, this views acronym-like words.

## Copy controls
The following controls influence the copying of text.

**Copy complete list to clipboard**. This copies the entire list to the clipboard.
This list is automatically copied to the clipboard by default each time a different View criterion is selected. 
However, the clipboard may change after the list is initially run.
This allows users to re-copy the list.<br>
**Copy selected word clipboard**. this selects an individual word. Highlight the intended word and select this button.<br>
**Allow copy to clipboard**. This check box controls copying to the clipboard.<br>
If selected, lists or words will be copied to the clipboard according the behavior outline earlier.<br>
If not selected, no list or word is copied to the clipboard.

## Caveats
*OpenAPI_Spellchecker* is offered and used as is.
While I did test it, you may find limitations and problems.
Feel free to report any comments, questions, and concerns, including bugs, to me.
My email is*robert@writeonce.org*
I will look into them.



