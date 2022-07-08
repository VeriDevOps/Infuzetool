# Infuzetool

Infuze test generator and fault localizer tool implemented using metamorphic testing and spectrum based fault localization techniques.

Infuze tool has two main parts : 
•	Test generator : Seed input and Morphed input generator for metamorphic testing 
•	Fault Localizer : Fault report and Annotated CFG generator for vulnerability localization

Test generator : 
Usage: Metamorphic testing uses a metamorphic relation defined between the inputs and outputs of multiple executions of the system under test.  Test generator takes the execution log traces of the system under test and generates as output the seed input file for the source test case and the morphed input files for the number of follow-up tests designed for the metamorphic testing process. 

Input: Execution log file of the system under test

Output: Seed input file for source test case
        Morphed input file for follow-up test1 (random approach)
        Morphed input file for follow-up test2 (guided approach)

Fault localizer :
Usage: Automatic vulnerability localization using Infuze fault localizer tool can help developers to visualize and identify the suspicious program parts and, therefore, fix the discovered faults /vulnerabilities through the metamorphic testing approach. The vulnerability localization process is to automatically identify the program parts at which the root cause of the fault is present. Our approach generates a CFG that enables the developer/programmer to visualize the difference in the execution paths between the successful and failed tests and a fault report that contains the program part with statements and corresponding line numbers. 

Input: Source code, Instrumented code, Test suite 

Output: Annotated Control Flow Graph , Fault Report
