# Intro To AI - Practice Problems - Phase 1

These problems and scenarios are to practice writing prompts for generative AI
tools. This could include generating code and text. You will also need to
generate local tests to help you verify your results meet the requirements.

****Which AI tool you decide to use is left to your discretion.**

Feel free to rewrite the skeleton code to better suit your needs and aid your
prompts.

## Problem 01 - A shortest path breadth first search

Your objective is to solve and test the graph problem to find the shortest path
of a graph represented by an adjacency list in **01-a-shortest-path-bfs.js**.

Consider combining the need for tests within a single prompt.

## Problem 02 - Binary search algorithm

Your objective is to generate and test the binary search algorithm in
**02-binary-search.js** in two different versions, both recursively AND
iteratively.

Challenge yourself by seeing if you can get the AI tool to generate both
recursive and iterative solutions with example test cases from a single prompt.

## Problem 03 - Permutations

Your objective is to convert the following JavaScript solution code into Python
in **03-permutations.py** along with local tests to verify it performs as
expected.

Additionally, write a prompt to give a walkthrough of the functioning code.

Consider writing a couple of alternative prompts for a walkthrough of the code
to see if you get different or more useful outputs.

```js
const permutations = (array) => {
  if (array.length <= 1) return [array];

  let first = array.shift();
  let perms = permutations(array);
  let allPerms = [];

  for (let i = 0; i < perms.length; i++) {
    let subPerm = perms[i];

    for (let j = 0; j <= subPerm.length; j++) {
      let left = subPerm.slice(0, j);
      let mid = [first];
      let right = subPerm.slice(j);

      allPerms.push(left.concat(mid).concat(right));
    }
  }

  return allPerms;
};
```

## Problem 04 - Dynamic programming

Your objective is to write a prompt to generate a dynamic programming example,
including a walkthrough of the functioning example code. The walkthrough should
include an explanation of why dynamic programming is useful in this case.

Capture the code and notes in **04-dynamic-programming.js**.

Consider doing some research of an article to include as a reference for the
prompt or to use as a basis for an alternative example.

## Problem 05 - Regex

Your objective is to write a prompt to generate a regular expression (regex) to
capture the requirements listed below. Generate a test to verify your code. Use
the provided file **05-regex.js** to record your results.

- A string that starts with a capital letter.
- A string that ends with a period.
- A string that contains a word that is 5 letters long and starts with a vowel.

Additionally, write a prompt to give a walkthrough of the functioning regex.

## Problem 06 - Seed data

Your objective is to write a prompt to generate seed data. You can use this as
an opportunity to generate seed for a project you are working on, OR you may
utilize the scenario below for experimentation.

Note, the file type provided is JSON (**06-seed-data.json**).

Aim for:

- At least 5 fields.
- At least 3 different data types.

Choose one of the examples of seed data subjects could be:

- Data of individuals.
- Data of books.
- Data of animals.
- Data of cars.

Consider writing a couple of alternative prompts for generating seed data to
see if you get different or more interesting outputs.

## Review and next steps

This is a good time review what you found effective and what caused you issues.
Learning how to utilize these AI tools will not happen immediately but the only
way to get better with them is to dive in and iteratively experiment!

As you reflect on what you tried, consider how the prompts you used might help
you build a full stack project! Make some notes for future reference.

When you have completed these problems, move onto the next phase.
