# Merge-JSON
Combine two JSON files into one

A simple Python application that combines two JSON files into one. This tool reads two input JSON files, merges their contents, and outputs the combined data to a new JSON file.

## Features

- Combines two JSON files.
- Handles key conflicts by prioritizing the second file's values.
- Outputs the combined JSON in a human-readable format.

## Requirements

- Python 3.12 or later

## Installation

1. Clone the repository or download the source code.
2. Ensure you have Python 3.12 installed on your machine.

## Usage

Run the script from the command line with the following syntax:

```bash
python combine_json.py

*** Example JSON files are included in the project named file1.json and file2.json

Enter the name of the first JSON file: file1.json
Enter the name of the second JSON file: file2.json
Enter the name for the output JSON file: output.json

Would you like to create a container object for the merged data? (yes/no):
yes

Enter the name for the container object:
person

Merged JSON data has been written to output.json




---------------------------------------------------------------
#Example Inputs


file1.json

{
    "name": "Alice",
    "age": 30,
    "country": "Switzerland"
}


file2.json

{
    "name": "Bob",
    "age": 25,
    "country": "USA"
}


#Example Expected Output

{
    "name": "Bob",
    "age": 25,
    "city": "New York",
    "country": "USA"
}
