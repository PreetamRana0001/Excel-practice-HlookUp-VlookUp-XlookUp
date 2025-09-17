# 🔎 Excel Lookup Functions (VLOOKUP + XLOOKUP)

This repository demonstrates how to use **VLOOKUP** and **XLOOKUP** in Excel to search and retrieve data from a table.

```excel
=VLOOKUP(101, A2:C20, 2, FALSE) 
// Searches for value 101 in the first column of A2:C20
// Returns the value from column 2 in the same row
// FALSE → Exact match required

=VLOOKUP("Apple", A2:D20, 4, TRUE) 
// Searches for "Apple" in the first column of A2:D20
// Returns the value from column 4
// TRUE → Approximate match (data must be sorted)

=XLOOKUP(101, A2:A20, B2:B20, "Not Found") 
// Looks for 101 in column A
// Returns corresponding value from column B
// If not found → shows "Not Found"

=XLOOKUP("Apple", B2:B20, D2:D20, "No Match", 0, -1) 
// Looks for "Apple" in column B
// Returns corresponding value from column D
// If not found → shows "No Match"
// 0 → Exact match, -1 → Search from bottom to top
