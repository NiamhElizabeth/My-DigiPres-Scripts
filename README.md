# My-DigiPres-Scripts
A collection of scripts to aid my digital preservation activities.

## Usage

### batchmd5.py
This script will create an MD5 manifest file for each digital file located within a directory. The default output directory is the current working directory, however there is an option to specify the output directory with the ‘-o’ argument. If the directory doesn’t exist, it will be created.

Usage with option to specify the output directory:

``
batchmd5.py /path/to/input_directory -o /path/to/output_directory
``

### md5.py
This script will create an MD5 manifest file for a digital file. The default output directory is the current working directory, however there is an option to specify the output directory with the ‘-o’ argument.

Usage with option to specify the output directory:

``
md5.py /path/to/input_file -o /path/to/output_directory
``

### validate.py
This script will validate an MD5 file or directory containing a batch of MD5 files against corresponding file or files. The MD5 input may be in a file or directory form whereas the corresponding file(s) must be in the form of a directory. 

The command-line will display the validation results, indicating whether each MD5 file is valid or invalid. At the end of the batch validation, a summary will be printed showing the total count of files validated.

Usage:

``
validate.py /path/to/input_file /path/to/corresponding_directory
``

``
validate.py /path/to/input_directory /path/to/corresponding_directory
``
