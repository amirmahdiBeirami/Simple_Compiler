<!-- START OF README -->

# Computer Design Final Project

Welcome to the **Computer Design Final Project** repository! This project is designed to help students gain hands-on experience with building a Lexer and Syntax Analyzer for a programming language defined by a custom grammar.

## Project Overview

### Language Grammar

Below is the grammar you will be implementing:

```plaintext
<S> => Program <VARS> <BLOCKS> end
<VARS> => Var Identifier; <VARS> | Epsilon
<BLOCKS> => Start <STATES> End
<STATES> => <STATE> <M_STATES>
<STATE> => <BLOCKS> | <IF> | <IN> | <OUT> | <ASSIGN> | <LOOP>
<M_STATES> => <STATES> | Epsilon
<OUT> => Print ( <EXPR> ) ;
<IN> => Read ( Identifier ) ;
<IF> => If ( <EXPR> <O> <EXPR> ) { <STATE> }
<LOOP> => Iteration ( <EXPR> <O> <EXPR> ) { <STATE> }
<ASSIGN> => Put Identifier = <EXPR> ;
<O> => < | > | ==
<EXPR> => <EXPR> + <R> | <EXPR> - <R> | <R>
<R> => Identifier | Integer
```


You are required to implement:
- **Lexer**: To tokenize the input program based on the grammar.
- **Syntax Analyzer**: To parse the tokenized input and validate it against the grammar rules.

## How to Participate

1. **Fork this Repository**:
   - Click the "Fork" button on the top right of this repository to create your own copy.

2. **Clone Your Fork**:
   - Clone your forked repository to your local machine:
     ```bash
     git clone https://github.com/Crisiroid/Simple_Compiler.git
     ```

3. **Create Your Project**:
   - Add your implementation files to the `src` directory in your forked repository.

4. **Commit Your Work**:
   - Commit your changes with meaningful commit messages:
     ```bash
     git add .
     git commit -m "Added Lexer and Syntax Analyzer implementation"
     ```

5. **Push to Your Fork**:
   - Push your changes to your forked repository:
     ```bash
     git push origin main
     ```

6. **Create a Pull Request**:
   - Navigate to the original repository.
   - Click the "New Pull Request" button.
   - Provide a description of your implementation and submit the pull request.

## Directory Structure

```plaintext
.
├── README.md        # Project instructions
├── Project/             # Directory for your implementation
│   ├── StudentNumber/    # Your Student Number

```

## Submission Guidelines

- Your project must be implemented in **C++**.
- Ensure your code is well-documented and includes comments explaining key parts of your logic.
- Include test cases in your `main.cpp` file to demonstrate the correctness of your Lexer and Syntax Analyzer.
- Follow the grammar strictly when implementing your Lexer and Syntax Analyzer.

### The pull request must include:
1. A brief description of your implementation.
2. Instructions on how to compile and run your project.

---

## Important Notes

- **Deadline**: All pull requests must be submitted before the project deadline. Late submissions will not be accepted.
- **Plagiarism**: Any copied or plagiarized work will result in disqualification.
- **Collaboration**: You are encouraged to discuss concepts with your peers, but the implementation must be your own.

---

## Getting Help

If you have any questions or need assistance, feel free to:
- Contact me at [csiroid@gmail.com](mailto:csiroid@gmail.com).
- Open an issue in this repository with your query.

---

**Happy coding and best of luck with your project!**



