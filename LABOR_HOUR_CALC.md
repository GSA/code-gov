# Labor Hour Calculation

To assist agencies in calculating labor hours, the [Code.gov](https://www.code.gov) team recommends agencies utilize Count Lines of Code (CLOC).

## Process

The process to calculate labor hours with CLOC follows.

1. Determine code repository where labor hours are to be calculated. This can be a public or private repository where the current code base resides.

2. Go to [CLOC](https://github.com/AlDanial/cloc) and download the desired software package or use the CLOC [website](https://codetabs.com/count-loc/count-loc-online.html) and point to a repository.

3. Capture the output of labor hours for the project and report it through your agency’s code.json file.

## Example

Here is an example on calculating labor hours with the GSA CTO [website](https://tech.gsa.gov/).

1. GSA begins with loading CLOC on the local machine and running it through the command line in Terminal with a result of 16,603 lines of code.

2. 16,603 is entered for labor hours in the code.json file.

## Disclaimer

This is not official guidance; rather we are providing this summary as a helpful resource for agencies to consider when calculating labor hours as part of each agency’s Code.json file. The Code.gov team recognizes that there are multiple ways to calculate labor hours and the process may be initially difficult for multiple reasons (e.g., undocumented labor hours, project changes over time, different contract types, various contractors). However, the team has tested various models and determined that, in order to identify a current baseline, an industry-recognized approach is to either calculate labor hours based on function points or lines of code. The solution offered was developed by software engineering experts and has been tested by agencies working with the Code.gov team with a high level of confidence. It is within each agency’s discretion to determine the approach that is most appropriate for their software inventory.
