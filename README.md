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

## Running Description_Finder
To run *OpenAPI_Spellchecker*,
1. Double click the application **OpenAPI_Spellchecker.exe**.
It opens to the *OpenAPI_Spellchecker* window.

## Operations
To get a list of descriptions:
1. Select **Open OpenAPI file**. This displays an open file dialog.
1. Navigate to, and then select the target OpenAPI source file.
1. Select **Open**. This opens the file and starts its processing. 
This may take a moment depending on the file size and internal complexity.

By default, the descriptions are automatically copied to the clipboard.
Without any additional involvement with the application, you can paste the clipboard into another document.
For example, this may be in Microsoft Word or as any text file.

The application shows the OpenAPI document's structure as tree view of all the paths. 
Any path may be expanded by clicking on it.
* Multiple clicks may be needed to fully traverse a branch.
* Clicking an open branch closes it.
* Multiple branches any be open at the same time.

The tree view provides no additional functionality other than being able to visually see the field structures with an endpoint.
You cannot get the descriptions for a specific branch of field.

## The Buttons

**Open OpenAPI file**. This selects and opens an OpenAPI source file. Once selected, the processing is automatic. This includes copying the descriptions to the clipboard. No additional action is required.

**Copy description to clipboard**. This copies the descriptions to the clipboard. This allows you to copy other items after first opening the application. The application is not re-run, nor is re-opening the source file required.

**Open all first levels**. This opens all first levels of each endpoint.

**Open all second levels**. This opens all second levels of each endpoint.

**Close all levels**. This closes all levels for each endpoint.

**Automatically copy to clipboard** (checkbox). This sets the default capability for automatically copying descriptions to the clipboard. There may instances when you want to see the field structures but not copy descriptions to the clipboard.<br>
* If checked, descriptions are copied to the clipboard.<br>
* If unchecked, descriptions are copied to the clipboard.

## Caveats
*Description_Finder* is offered and used as is.
While I did test it, you may find limitations and problems.
Feel free to report any comments, questions, and concerns, including bugs, to me.
I will look into them.


