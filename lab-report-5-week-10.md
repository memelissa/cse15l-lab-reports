# Lab Report 5 (Week 10)

## How I Found the Test Differences

In order to find the tests with different results by using the command, `diff markdown-parse/out.txt MarkdownParse/results.txt`.  By using this command, it returns all the differences between `results.txt` of my `MarkdownParse.java` and results of the `markdown-parse` repository that was given to us.

## Test 1: File 495

### Preview Image Output:
![File495](495.png)

### Output of Both Implementations:
![File494](494diff.png)






## Test 2: File 494

### Preview Image Output:
![File494](494.png)

### Output of Both Implementations:
![File494](494diff.png)

For `test-files/494.md`, both of the implementations resulted in the incorrect output, with my implementation producing the output of `[\(foo\]` and the other giving `[\(foo\)]`. The correct output should be `[(foo)]`, therefore both are wrong. 

### Bug in Code:
![File494](494bug.png)

For my implementation, the bug in my code can be found when it is attempting to find the closing parentheses. As shown, the code will only find the first closing parantehses after the first opening parantheses, but fails to recognize multiple closing parantheses. The bug can be fixed with a change to the `openParen` and `closeParen`, and maybe a mathod that accounts for the values of each parantheses to ensure that each closing parantheses will be considered. 

