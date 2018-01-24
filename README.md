# lcov-llvm-function-mishit-filter
Python 3 script to filter lcov output and remove function signature lines that are never report as hit

# What's This?
The lcov test coverage utility is designed to work with gcc and has some issued with running on binaries generated by the llvm compiler. One of these issues is that function signatures are output as lines that should be hit. However, while the binary is running those function signature lines are never registered as hit. Here's a simple python script to filter those lines from the lcov output.

# How To?
 `remove-function-lines.py lcov_output.info cleaned_output.info`
 
# More Info
 Check out this issue from the lcov project
 https://github.com/linux-test-project/lcov/issues/30
 
