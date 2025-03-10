# 2019-05 Online Test Results
This location is for test results (test TDs and manual assertion declarations
given in CSV files) that will be used to generate 
the draft Implementation Report after CR transition and prior to PR transition. 

Current version of Implementation Report: https://github.com/w3c/wot-thing-description/blob/master/testing/report.html

See the comments at the start of `update.sh` for instructions on how the
input files should be organized.  Generally speaking, inputs (both TDs and 
manual assertions in CSV files) should go in 
the `interop` and `inputs` directories, grouped into subdirectories for each
reporting organization and implementation.  Running `update.sh` will then run
the assertion tester in `thingweb-playground`.  The assertion tester is included as
a recursive git repo under `testing/tools` in this repo. 
Running the `update.sh` script will update the files in `outputs`. 
The top-level CSV files in `outputs` should then be copied to 
`wot-thing-directory/testing/results` before generating the Implementation
Report (see `wot-thing-directory/README.md` for instructions on how to do that).
