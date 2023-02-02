# csv2json

This script is used by the `gh` command-line to help convert a **CSV** file into a **JSON** file/object.
This is useful if you have a large csv export of data, and need to ingest it into a system that requires a JSON object.

## PREREQS

You need to have the following to run this script successfully:

- **jq** installed on the machine running the query

## Input file

The `input file` should be in the format:

```csv
HEADER1,HEADER2,HEADER3,etc
value1,value2,value3,etc
value1,value2,value3,etc
value1,value2,value3,etc
```

The script will read the input file line by line and convert it into a JSON object. It will also skip over empty values and headers to produce a valid JSON object.

## Usage

`gh csv2json --file possum_statistics.csv --output possum_statistics.json`

### Output

```bash
gh csv2json --file possum_statistics.csv --output possum_statistics.json

######################################################
######################################################
############# csv2json conversion tool ###############
######################################################
######################################################

Output will be written to:[data.json]

Warning: This script will overwrite any existing file with the same name as the output file.
This script could possibly take a while to run, depending on the size of the csv file.
This script will not validate the csv file, so please ensure it is in the correct format.
This script could take up a large section of memory if you do NOT choose to output to a file as it will hold the entire json object in memory.

Parsing Line: [1] of [64]
Parsing Line: [2] of [64]
Parsing Line: [3] of [64]
Parsing Line: [4] of [64]
Parsing Line: [5] of [64]
Parsing Line: [6] of [64]
Parsing Line: [7] of [64]
Parsing Line: [8] of [64]
Parsing Line: [9] of [64]
Parsing Line: [10] of [64]
Parsing Line: [11] of [64]
Parsing Line: [12] of [64]
Parsing Line: [13] of [64]
Parsing Line: [14] of [64]
Parsing Line: [15] of [64]
Parsing Line: [16] of [64]
Parsing Line: [17] of [64]
Parsing Line: [18] of [64]
Parsing Line: [19] of [64]
Parsing Line: [20] of [64]
Parsing Line: [21] of [64]
Parsing Line: [22] of [64]
Parsing Line: [23] of [64]
Parsing Line: [24] of [64]
Parsing Line: [25] of [64]
Parsing Line: [26] of [64]
Parsing Line: [27] of [64]
Parsing Line: [28] of [64]
Parsing Line: [29] of [64]
Parsing Line: [30] of [64]
Parsing Line: [31] of [64]
Parsing Line: [32] of [64]
Parsing Line: [33] of [64]
Parsing Line: [34] of [64]
Parsing Line: [35] of [64]
Parsing Line: [36] of [64]
Parsing Line: [37] of [64]
Parsing Line: [38] of [64]
Parsing Line: [39] of [64]
Parsing Line: [40] of [64]
Parsing Line: [41] of [64]
Parsing Line: [42] of [64]
Parsing Line: [43] of [64]
Parsing Line: [44] of [64]
Parsing Line: [45] of [64]
Parsing Line: [46] of [64]
Parsing Line: [47] of [64]
Parsing Line: [48] of [64]
Parsing Line: [49] of [64]
Parsing Line: [50] of [64]
Parsing Line: [51] of [64]
Parsing Line: [52] of [64]
Parsing Line: [53] of [64]
Parsing Line: [54] of [64]
Parsing Line: [55] of [64]
Parsing Line: [56] of [64]
Parsing Line: [57] of [64]
Parsing Line: [58] of [64]
Parsing Line: [59] of [64]
Parsing Line: [60] of [64]
Parsing Line: [61] of [64]
Parsing Line: [62] of [64]
Parsing Line: [63] of [64]
Parsing Line: [64] of [64]

######################################################
The script has completed
######################################################
Total time to run script: [2] seconds
Output file:[data.json]
```