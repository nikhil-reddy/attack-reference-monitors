# attack-reference-monitors
Goal: Attack other students' reference monitors.

Create multiple test cases:

   1. One test per issue (if you add multiple tests within the same program (file) and one of them is wrong, you will lose points for all of them)
   2. Must output only when a bug is found! (outputs can be exceptions or log statements)

Your test case should not output anything if the security layer passes it. It should print appropriate error message only if the security layer fails in terms of either of the following:

   1. Accuracy bug
   2. Security bug

Note: Use the test cases attached to this assignment as examples, since the ones on the website will produce an output even when the security layer has no bugs.

   If your test is wrong, you will lose points!

Assignment instructions:

https://seattle.poly.edu/wiki/EducationalAssignments/SecureStoragePartTwo



How to run your tests on many reference monitors:

If you are using Mac or Linux, you can do something like the following:

Put all security layer and attack cases in the same directory you were using before to run single security layer and attack program. 

Then you can type the following in the bash shell to execute the testcases with the reference monitors:

for referencemonitor in reference_*;  do for testcase in netid_*.r2py; do python repy.py restrictions.default encasementlib.r2py $referencemonitor $testcase;  done;  done
