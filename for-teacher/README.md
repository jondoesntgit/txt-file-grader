# TEXT FILE GRADER for teachers

## Background

This is a shell script that implements awk for generating grade report sheets for multiple students in a class together.

I used this with my 7th and 8th math courses when I was volunteer teaching in Beirut Lebanon. I ran this program in a Dropbox, and shared the link of each students' outfile with the students so they could check their grades at any time.

## Usage

Create one text file for each category. Each assignment takes up one line. Make sure that student names are the same order in each file (I put them in alphabetically).

I would enter an "m" or "a" for absent students. These two would be counted as "0" in the gradebook.

For students who were exempt from the assignement, I would enter "x" and this would not affect their individual points possible.

When finished, run `program` and it will create the outfiles directory (if it does not already exist) and populate it with txt output files.

### Separating reports
I was able to generate a separate report for each grading point (GP#). 

A student report would show all assignments between two dates, labeled *yymmdd* both in the program and in the txt files.

A midterm or final report would only show entries from the test.txt file labeled "final" or "midterm"

### Limitations
Extra credit could be entered as when there were 0 possible points

Currently, there is no weighting supported by the program. Points possible in each category add, and points total in each category add. The final average is the total points scored divided by the total points possible.

## Examples

This repository shows some example grades from my year of teaching.
