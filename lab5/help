#!/bin/bash
echo "System memory parameter values:" >> report.txt
top n 1 -b | awk 'NR == 4 { print $4 " -total " $6  " -free " $8 " -used " $10 " -buff/cashe" }' >> report.txt
top n 1 -b | awk 'NR == 5 {print $3 " -total " $5  " -free " $7 " -used " $9 " -buff/cashe"}' >> report.txt
top -n 1 -b | grep -w 'mem' >> report.txt
top -n 1 -b | awk 'NR >= 8 && NR <= 12 {print $1}' >> report.txt
echo "" >> report.txt

