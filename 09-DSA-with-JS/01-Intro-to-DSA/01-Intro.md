<h2 align="center"> Intro To DSA </h2>


### What is Data Structure? 
- A data structure is a specific way of organizing, storing, and accessing data.

### What is Algorithm? 
- A set of instructions that tells a computer how to do something, or you can also say step-by-step solution of the problem is called algorithm.

---

### CHALLENGE 🎯

Create an array with 5 students names, after that create a function which takes 2 parameters (allStudents & studentName) iterate over all students and find that
specific user "studentName".

**HINT**: 
1. Create an array of 5 student names.

2. Write a function that:
- Takes two parameters: `allStudents` (array of names) and `studentName` (the name to find).
- Iterates over `allStudents`.
- If `studentName` is found, return `"Found: [name]".`
- If not found, return `"Not Found"`.

<details>
<summary><code>Solution</code></summary>

```javascript
// Step 1: Create an array of student names
const students = ["Aditi", "Rahul", "Meera", "Zaid", "Kabir"];

// Step 2: Function to find a student
function findStudent(allStudents, studentName) {
  for (let i = 0; i < allStudents.length; i++) {
    if (allStudents[i] === studentName) {
      return `Found: ${studentName}`;
    }
  }
  return "Not Found";
}

// Test Cases : Run test cases in your terminal 
console.log(findStudent(students, "Meera"));  // Output: Found: Meera
console.log(findStudent(students, "John"));   // Output: Not Found

```
</details>

---

### DEEP ANALYSIS 🔎

Q. What data structure is used to solve the above problem? 
```javascript 
// Data Structure 👇 : array 
const students = ["Aditi", "Rahul", "Meera", "Zaid", "Kabir"];
```


Q. What algorithm is used in the above problem? 
```javascript 
// Algorithm 👇 : for finding a specific Student
function findStudent(allStudents, studentName) {
  for (let i = 0; i < allStudents.length; i++) {
    if (allStudents[i] === studentName) {
      return `Found: ${studentName}`;
    }
  }
  return "Not Found";
}

```

---


### Why Do I Care ❓

The answer is simple. If you want to get good at these : 

- Efficient Problem Solving
- Stronger Coding Skills
- Algorithmic Awareness
- Interview Success
- Coding Confidence
- Efficiency Expert
- Improved Logical Thinking
- Future-Proof Your Skills
- Innovation Inspiration
- Lifelong Learning
- Critical Thinking Champion

You must understand how data works and become a great **Problem Solver**

---






