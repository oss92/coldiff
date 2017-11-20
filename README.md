# coldiff
## Usage
To find intersection between columns in 2 files
```bash
./coldiff -i file_one.csv,file_two.csv
```

Specify a column number
```bash
# compares column number 3 of file_one with column number 2 of file_two
./coldiff -i file_one.csv:3,file_two.csv:2
```

To find difference between 2 files
```bash
# Outputs what is IN file_one and NOT IN file_two
./coldiff -i file_one.csv:3 -n file_two.csv:2

# Outputs what is IN file_one and NOT IN file_two
# Plus what is IN file_three and NOT IN file_two
./coldiff -i file_one.csv:3,file_three.csv -n file_two.csv:2
```
