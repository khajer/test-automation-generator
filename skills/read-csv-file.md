---
name: read-csv-file
description: Reads and summarizes a CSV file using a nodejs typescript. Use when a user provides a .csv file and wants to view its content or analysis.
allowed-tools: "Read, Bash(node:read_csv_data.ts)"
version: 1.0.0
license: MIT
author: AI Agent
tags: ["csv", "data-analysis", "node", "read"]
---

## How to use the `read-csv-file` skill

1. The user provides a path to a CSV file.
2. The AI must execute the helper script `read_csv_data.ts` via bash, passing the file path as an argument.
3. The AI should analyze the output provided by the script to answer the user's questions or present the summary.

**Example execution:**
`bash python read_csv_data.ts "path/to/user_data.csv"`
