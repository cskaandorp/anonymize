# Anonymize UU

This description can be found [on GitHub here](https://github.com/cskaandorp/anonymize)

Anonymize_UU facilitates the substittion of keywords or patterns within a file tree or zipped archive. In case of a zip-file, anonymize_UU will unzip the archive in a temp directory and starts it work from there.It recursively traverses the tree, reads supported files and subsitutes any found pattern or keyword. Besides contents, anomize_UU will substitue keywords/patterns in file/folder-paths as well.

As of now, Anonymize_UU supports text-based files, like .txt, .html, .json and .csv. UTF-8 encoding is assumed. Besides text files, Anonymize_UU is also able to handle nestes zip archives. These archives will be unpacked in a temp folder, processed and zipped again.

The result will be either a copied or replaced version of the original file-tree with all substitutions made.

## Installation

`$ pip install anonymize_UU`

## Usage

Import the Anomymize class in your code and create an anonymization object like this:

```
from anonymize import Anonymize

anonymize = Anonymize('/Users/casper/Desktop/keys.csv')
```