# Ex.No: 9 Logic Programming – Computer Maintenance Expert System
## DATE: 16.09.2023
## REGISTER NUMBER : 2122210400056
## AIM: Write a Prolog program to build a computer maintenance expert system.

## Algorithm:
Start the program.
Write the rules for each fault in computer.
If system have printing problem, missing dots and no uniform printing then system fault on printer head.
If system have not printing, missing dots and spread inks then system fault on ribbon
If system have not printing, paper jam and out of paper then system fault on paper stuck in printer
Similarly define rules for all faults.
Define facts for system problems.
Find the fault of computer by passing query to system.
## program:
```
fault(printer_head) :-
problem(not_printing),
problem(missing_dots),
problem(nonuniform_printing).
fault(ribbon) :-
problem(not_printing),
problem(missing_dots),
problem(spread_ink).
fault(paper) :-
problem(not_printing),
problem(paper_jam),
problem(out_of_paper).
fault(motherboard) :-
problem(long_beep),
problem(short_beep).
fault(hard_disc) :-
problem(two_short_beeps),
problem(blank_display).
problem(not_printing).
problem(missing_dots).
problem(spread_ink).
problem(two_short_beeps).
problem(blank_display).
```
## Output:
![image](https://github.com/HibaRajarajeswari/COMPUTER-MAINTENANCE/assets/129970809/7d0ead29-0c9a-48d8-9fe9-6ad5788e4d05)


## Result:
Thus the simple omputer maintenance expert system was built sucessfully.
