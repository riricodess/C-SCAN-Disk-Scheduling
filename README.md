# C-SCAN-Disk-Scheduling

This repository contains a C program implementing the **C-SCAN (Circular SCAN) Disk Scheduling Algorithm** for Operating Systems Experiment 13.

## Aim
To implement the C-SCAN disk scheduling algorithm and calculate the disk head movement for a given set of disk requests.

## Input Details
- **Initial disk head position:** 53
- **Last track:** 199
- **Disk requests:** 98, 183, 37, 122, 14, 124, 65, 67

## Files Included
- `cscan.c` – C program implementing the C-SCAN algorithm.
- `cscan_output.txt` – Program output.
- `cscan_output.png` – Output displayed as an image.

## Requirements
- GCC compiler
- Linux terminal or Ubuntu environment

## Compilation and Execution

Compile the program:

```bash
gcc cscan.c -o cscan
```

Run the program:

```bash
./cscan
```

## Expected Output

```text
Order: 53 -> 65 -> 67 -> 98 -> 122 -> 124 -> 183 -> 199 -> 0 -> 14 -> 37
Total seek = 382
```

## Real-World Application
This algorithm can be used to understand disk request scheduling in systems that process multiple file requests, such as an online examination portal handling student submissions.

## Conclusion
The C-SCAN disk scheduling algorithm services requests in one direction, moves to the last track, returns to track 0, and continues servicing the remaining requests. For the given input, the total disk head movement is **382 tracks**.
