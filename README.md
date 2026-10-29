# Web Application Development Laboratory

**End Semester Practical Examination — November/December 2026**  
**Course:** Web Application Development Laboratory  
**Department:** Artificial Intelligence and Data Science (AI&DS)  
**Technologies:** HTML5, CSS3, JavaScript

This repository contains 20 beginner-friendly web development practical assignments. Each experiment can be run locally in a browser. The examples demonstrate HTML structure, forms, styling, navigation, JavaScript validation, DOM manipulation, and interactive applications.

## Getting Started

1. Clone or download the repository.
2. Open the folder for the experiment you want to run.
3. Open `index.html` in a web browser (or use VS Code Live Server).
4. For Experiment 6, keep `index.html` and `style.css` in the same folder.

## Suggested Repository Structure

```text
web-application-development-lab/
├── README.md
├── experiment-01/index.html
├── experiment-02/index.html
├── experiment-03/index.html
├── experiment-04/index.html
├── experiment-05/index.html
├── experiment-06/index.html
├── experiment-06/style.css
├── experiment-07/index.html
├── experiment-08/index.html
├── experiment-09/index.html
├── experiment-10/index.html
├── experiment-11/index.html
├── experiment-12/index.html
├── experiment-13/index.html
├── experiment-14/index.html
├── experiment-15/index.html
├── experiment-16/index.html
├── experiment-17/index.html
├── experiment-18/index.html
├── experiment-19/index.html
└── experiment-20/index.html
```

## Experiment Index

| No. | Experiment | Concepts |
|---:|---|---|
| 01 | College Department Profile | Headings, paragraphs, text formatting |
| 02 | Job Listing Webpage | HTML tables |
| 03 | Student Registration Form | Forms, inputs, dropdowns, radio buttons |
| 04 | Campus Interview Registration | Forms, file input, checkboxes |
| 05 | College Website Navigation | Anchor links, internal CSS |
| 06 | Department Website Styling | Inline, internal, external CSS |
| 07 | Online Bookstore | CSS backgrounds, borders, spacing |
| 08 | Navigation Menu | CSS hover effects |
| 09 | Examination Registration Validation | JavaScript form validation |
| 10 | Email and Phone Validation | Regular expressions |
| 11 | Student Marks Update | DOM manipulation |
| 12 | Character Counter | Input events |
| 13 | Shopping Cart Total | Dynamic calculations |
| 14 | Login Form Validation | Conditional statements |
| 15 | Student Dashboard | Event handling, dynamic content |
| 16 | Tic-Tac-Toe | Game logic, arrays, DOM |
| 17 | Sudoku Solver | Backtracking algorithm |
| 18 | Unit Converter | Arithmetic, selection controls |
| 19 | Basic Calculator | JavaScript functions |
| 20 | Calculator and Converter | HTML, CSS, JS integration |

---

## Experiment 01 — College Department Profile

**Aim:** Create a department profile page using headings, paragraphs, bold/italic text, and a highlighted announcement.

**File:** `experiment-01/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>College Department</title></head>
<body>
  <h1>ABC College of Engineering</h1>
  <h2>Department of AI & DS</h2>
  <p>Welcome to our department.</p>
  <h3>About Department</h3>
  <p>We provide quality education in Artificial Intelligence and Data Science.</p>
  <b>Vision:</b><p>To become a center of excellence.</p>
  <i>Mission: To develop skilled engineers.</i>
  <h3>Announcements</h3>
  <mark>Semester Examination starts soon!</mark>
</body>
</html>
```

**Expected output:** Department information with a highlighted announcement.

## Experiment 02 — Job Listing Webpage

**Aim:** Display job titles, locations, salaries, and availability in a table.

**File:** `experiment-02/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Job Portal</title></head>
<body>
  <h1>Job Opportunities</h1>
  <table border="1" cellpadding="10">
    <tr><th>Job Title</th><th>Location</th><th>Salary</th><th>Status</th></tr>
    <tr><td>Web Developer</td><td>Chennai</td><td>30000</td><td>Available</td></tr>
    <tr><td>Python Developer</td><td>Bangalore</td><td>40000</td><td>Available</td></tr>
    <tr><td>Data Analyst</td><td>Coimbatore</td><td>35000</td><td>Closed</td></tr>
  </table>
</body>
</html>
```

## Experiment 03 — Student Registration Form

**Aim:** Collect student details using HTML form controls.

**File:** `experiment-03/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Student Registration</title></head>
<body>
  <h2>Student Registration Form</h2>
  <form onsubmit="alert('Registration submitted'); return false;">
    Name: <input type="text" required><br><br>
    Register Number: <input type="text" required><br><br>
    Email: <input type="email" required><br><br>
    Phone: <input type="tel" required><br><br>
    Department: <select><option>AI & DS</option><option>CSE</option><option>IT</option></select><br><br>
    Gender: <label><input type="radio" name="gender" required>Male</label>
    <label><input type="radio" name="gender">Female</label><br><br>
    <input type="submit" value="Register"> <input type="reset" value="Clear">
  </form>
</body>
</html>
```

## Experiment 04 — Campus Interview Registration

**Aim:** Create a campus interview application form with resume upload and skill selection.

**File:** `experiment-04/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Campus Interview</title></head>
<body>
  <h2>Campus Interview Registration</h2>
  <form onsubmit="alert('Application submitted'); return false;">
    Student Name: <input type="text" required><br><br>
    Email: <input type="email" required><br><br>
    Phone: <input type="tel" required><br><br>
    Department: <select><option>AI & DS</option><option>CSE</option><option>ECE</option></select><br><br>
    Resume: <input type="file" required><br><br>
    Skills:<br>
    <label><input type="checkbox">Python</label>
    <label><input type="checkbox">Java</label>
    <label><input type="checkbox">HTML</label><br><br>
    <input type="submit" value="Apply">
  </form>
</body>
</html>
```

## Experiment 05 — College Website Navigation

**Aim:** Build a single-page college website with navigation links.

**File:** `experiment-05/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>College Website</title>
  <style>
    body { font-family: Arial; text-align: center; }
    nav { background: navy; padding: 15px; }
    nav a { color: white; margin: 15px; text-decoration: none; }
    section { padding: 30px; }
  </style>
</head>
<body>
  <h1>ABC Engineering College</h1>
  <nav>
    <a href="#home">Home</a><a href="#department">Departments</a>
    <a href="#faculty">Faculty</a><a href="#courses">Courses</a>
    <a href="#contact">Contact</a>
  </nav>
  <section id="home"><h2>Home</h2><p>Welcome to our college.</p></section>
  <section id="department"><h2>Departments</h2><p>AI & DS, CSE, ECE, IT</p></section>
  <section id="faculty"><h2>Faculty</h2><p>Experienced teaching staff.</p></section>
  <section id="courses"><h2>Courses</h2><p>B.Tech and M.Tech</p></section>
  <section id="contact"><h2>Contact</h2><p>Email: college@example.com</p></section>
</body>
</html>
```

## Experiment 06 — Department Website Using CSS

**Aim:** Demonstrate inline, internal, and external CSS.

**File:** `experiment-06/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Department Website</title>
  <link rel="stylesheet" href="style.css">
  <style>h1 { text-align: center; }</style>
</head>
<body>
  <h1 style="color:blue;">AI & DS Department</h1>
  <div class="box"><h2>About Us</h2><p>Welcome to our department.</p></div>
  <div class="box"><h2>Courses</h2><p>Artificial Intelligence</p><p>Data Science</p></div>
</body>
</html>
```

**File:** `experiment-06/style.css`

```css
body { font-family: Arial; background-color: lightgray; }
.box { background-color: white; padding: 20px; margin: 20px;
       border: 2px solid blue; border-radius: 10px; }
```

## Experiment 07 — Online Bookstore

**Aim:** Style book cards using CSS backgrounds, borders, margins, and padding.

**File:** `experiment-07/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Online Bookstore</title>
  <style>
    body { background: lightblue; font-family: Arial; text-align: center; }
    .book { background: white; border: 2px solid black; padding: 20px;
            margin: 20px; display: inline-block; border-radius: 10px; }
    button { background: green; color: white; padding: 10px; }
  </style>
</head>
<body>
  <h1>Online Bookstore</h1>
  <div class="book"><h2>Python Programming</h2><p>Price: Rs. 500</p><button>Buy Now</button></div>
  <div class="book"><h2>Web Development</h2><p>Price: Rs. 600</p><button>Buy Now</button></div>
</body>
</html>
```

*The Buy Now buttons are visual demonstrations and do not process purchases.*

## Experiment 08 — Navigation Menu with Hover Effects

**Aim:** Create a navigation menu with CSS hover styling.

**File:** `experiment-08/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Navigation Menu</title>
  <style>
    body { font-family: Arial; }
    nav { background: black; padding: 20px; }
    nav a { color: white; padding: 15px; text-decoration: none; }
    nav a:hover { background: orange; color: black; }
  </style>
</head>
<body>
  <h1>Student Portal</h1>
  <nav><a href="#home">Home</a><a href="#about">About</a>
       <a href="#courses">Courses</a><a href="#contact">Contact</a></nav>
  <h2 id="home">Welcome</h2><p>Move your mouse over the menu.</p>
  <h2 id="about">About</h2><p>Student information portal.</p>
  <h2 id="courses">Courses</h2><p>Available courses.</p>
  <h2 id="contact">Contact</h2><p>Contact the college office.</p>
</body>
</html>
```

## Experiment 09 — Examination Registration Validation

**Aim:** Validate mandatory fields using JavaScript and the DOM.

**File:** `experiment-09/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Exam Registration</title></head>
<body>
  <h2>Exam Registration Form</h2>
  <form onsubmit="return validate()">
    Name: <input type="text" id="name"><br><br>
    Register Number: <input type="text" id="reg"><br><br>
    Email: <input type="email" id="email"><br><br>
    <input type="submit" value="Register">
  </form>
  <script>
    function validate() {
      let name = document.getElementById('name').value;
      let reg = document.getElementById('reg').value;
      let email = document.getElementById('email').value;
      if (!name.trim() || !reg.trim() || !email.trim()) {
        alert('All fields are mandatory');
        return false;
      }
      alert('Registration Successful');
      return false;
    }
  </script>
</body>
</html>
```

## Experiment 10 — Email and Phone Validation

**Aim:** Validate an email address and a 10-digit phone number.

**File:** `experiment-10/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Form Validation</title></head>
<body>
  <h2>Admission Form</h2>
  Email: <input type="text" id="email"><br><br>
  Phone: <input type="text" id="phone"><br><br>
  <button onclick="validate()">Submit</button>
  <p id="result"></p>
  <script>
    function validate() {
      let email = document.getElementById('email').value;
      let phone = document.getElementById('phone').value;
      let emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      let phonePattern = /^[0-9]{10}$/;
      if (!emailPattern.test(email)) alert('Invalid Email');
      else if (!phonePattern.test(phone)) alert('Invalid Phone Number');
      else document.getElementById('result').textContent = 'Registration Successful';
    }
  </script>
</body>
</html>
```

## Experiment 11 — Student Marks Update

**Aim:** Update displayed student marks dynamically.

**File:** `experiment-11/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Student Result</title></head>
<body>
  <h2>Student Result</h2>
  <p>Student Name: Arun</p>
  <p>Marks: <span id="marks">75</span></p>
  <button onclick="updateMarks()">Update Marks</button>
  <script>
    function updateMarks() {
      let marks = prompt('Enter New Marks:');
      if (marks === null) return;
      let value = Number(marks);
      if (marks.trim() === '' || !Number.isFinite(value) || value < 0 || value > 100)
        alert('Enter valid marks between 0 and 100');
      else document.getElementById('marks').textContent = value;
    }
  </script>
</body>
</html>
```

## Experiment 12 — Character Counter

**Aim:** Count characters as the user types or deletes text.

**File:** `experiment-12/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Character Counter</title></head>
<body>
  <h2>Feedback Form</h2>
  <textarea id="text" rows="5" cols="40" oninput="count()"></textarea>
  <p>Character Count: <span id="result">0</span></p>
  <script>
    function count() {
      document.getElementById('result').textContent =
        document.getElementById('text').value.length;
    }
  </script>
</body>
</html>
```

## Experiment 13 — Shopping Cart Price Calculation

**Aim:** Recalculate the total price when the quantity changes.

**File:** `experiment-13/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Shopping Cart</title></head>
<body>
  <h2>Online Shopping</h2>
  <p>Product: Laptop Bag</p><p>Price: Rs. 500</p>
  Quantity: <input type="number" id="qty" value="1" min="1" oninput="calculate()">
  <h3>Total Price: Rs. <span id="total">500</span></h3>
  <script>
    function calculate() {
      let qty = Number(document.getElementById('qty').value);
      document.getElementById('total').textContent =
        Number.isInteger(qty) && qty >= 1 ? qty * 500 : 'Invalid quantity';
    }
  </script>
</body>
</html>
```

## Experiment 14 — Login Form Validation

**Aim:** Validate demonstration username/password credentials on the client side.

**File:** `experiment-14/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Login Page</title></head>
<body>
  <h2>College Portal Login</h2>
  Username: <input type="text" id="username"><br><br>
  Password: <input type="password" id="password"><br><br>
  <button onclick="login()">Login</button>
  <p id="message"></p>
  <script>
    function login() {
      let user = document.getElementById('username').value;
      let pass = document.getElementById('password').value;
      document.getElementById('message').textContent =
        user === 'admin' && pass === '1234'
          ? 'Login Successful' : 'Invalid Username or Password';
    }
  </script>
</body>
</html>
```

**Demo credentials:** `admin` / `1234`. This is **not secure authentication**; real login requires a backend.

## Experiment 15 — Student Dashboard Navigation

**Aim:** Show dashboard content dynamically when navigation buttons are clicked.

**File:** `experiment-15/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Student Dashboard</title>
  <style>button { padding: 10px; margin: 5px; background: blue; color: white; }</style>
</head>
<body>
  <h2>Student Dashboard</h2>
  <button onclick="show('Attendance: 90%')">Attendance</button>
  <button onclick="show('Internal Marks: 85')">Internal Marks</button>
  <button onclick="show('Timetable: Monday to Friday')">Timetable</button>
  <button onclick="show('Course Materials Available')">Course Materials</button>
  <h3 id="result"></h3>
  <script>
    function show(message) {
      document.getElementById('result').textContent = message;
    }
  </script>
</body>
</html>
```

## Experiment 16 — Tic-Tac-Toe Game

**Aim:** Build a two-player Tic-Tac-Toe game with turn management, win/draw detection, and reset.

**File:** `experiment-16/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Tic Tac Toe</title>
  <style>
    body { text-align: center; font-family: Arial; }
    .board { display: grid; grid-template-columns: repeat(3, 80px); justify-content: center; }
    .cell { width: 80px; height: 80px; font-size: 30px; }
  </style>
</head>
<body>
  <h2>Tic Tac Toe</h2>
  <h3 id="status">Player X Turn</h3>
  <div class="board" id="board"></div><br>
  <button onclick="reset()">Reset</button>
  <script>
    let cells = Array(9).fill('');
    let player = 'X';
    let gameOver = false;
    const wins = [[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]];
    function draw() {
      let board = document.getElementById('board');
      board.innerHTML = '';
      cells.forEach((value, i) => {
        let btn = document.createElement('button');
        btn.className = 'cell';
        btn.textContent = value;
        btn.onclick = () => play(i);
        board.appendChild(btn);
      });
    }
    function play(i) {
      if (cells[i] !== '' || gameOver) return;
      cells[i] = player;
      if (wins.some(w => w.every(index => cells[index] === player))) {
        document.getElementById('status').textContent = 'Player ' + player + ' Wins!';
        gameOver = true;
      } else if (cells.every(c => c !== '')) {
        document.getElementById('status').textContent = 'Game Draw!';
        gameOver = true;
      } else {
        player = player === 'X' ? 'O' : 'X';
        document.getElementById('status').textContent = 'Player ' + player + ' Turn';
      }
      draw();
    }
    function reset() {
      cells = Array(9).fill('');
      player = 'X';
      gameOver = false;
      document.getElementById('status').textContent = 'Player X Turn';
      draw();
    }
    draw();
  </script>
</body>
</html>
```

## Experiment 17 — Sudoku Solver

**Aim:** Solve a valid Sudoku grid using a recursive backtracking algorithm.

**File:** `experiment-17/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Sudoku Solver</title>
  <style>
    body { text-align: center; }
    #board { display: grid; grid-template-columns: repeat(9, 35px); justify-content: center; }
    input { width: 30px; height: 30px; text-align: center; }
  </style>
</head>
<body>
  <h2>Sudoku Solver</h2>
  <div id="board"></div><br>
  <button onclick="solve()">Solve Sudoku</button>
  <p id="message"></p>
  <script>
    let board = document.getElementById('board');
    for (let i = 0; i < 81; i++) {
      let input = document.createElement('input');
      input.type = 'number'; input.min = '1'; input.max = '9';
      board.appendChild(input);
    }
    function valid(grid, row, col, num) {
      for (let i = 0; i < 9; i++)
        if (grid[row][i] === num || grid[i][col] === num) return false;
      let r = Math.floor(row / 3) * 3;
      let c = Math.floor(col / 3) * 3;
      for (let i = r; i < r + 3; i++)
        for (let j = c; j < c + 3; j++)
          if (grid[i][j] === num) return false;
      return true;
    }
    function solver(grid) {
      for (let r = 0; r < 9; r++) {
        for (let c = 0; c < 9; c++) {
          if (grid[r][c] === 0) {
            for (let n = 1; n <= 9; n++) {
              if (valid(grid, r, c, n)) {
                grid[r][c] = n;
                if (solver(grid)) return true;
                grid[r][c] = 0;
              }
            }
            return false;
          }
        }
      }
      return true;
    }
    function solve() {
      let inputs = document.querySelectorAll('#board input');
      let grid = [];
      for (let r = 0; r < 9; r++) {
        grid[r] = [];
        for (let c = 0; c < 9; c++) {
          let value = inputs[r * 9 + c].value;
          if (value !== '' && !/^[1-9]$/.test(value)) {
            alert('Enter digits 1 to 9 only'); return;
          }
          grid[r][c] = value === '' ? 0 : Number(value);
        }
      }
      for (let r = 0; r < 9; r++) {
        for (let c = 0; c < 9; c++) {
          if (grid[r][c] !== 0) {
            let n = grid[r][c]; grid[r][c] = 0;
            if (!valid(grid, r, c, n)) { alert('Invalid Sudoku'); return; }
            grid[r][c] = n;
          }
        }
      }
      if (solver(grid)) {
        inputs.forEach((input, i) => {
          input.value = grid[Math.floor(i / 9)][i % 9];
        });
        document.getElementById('message').textContent = 'Sudoku Solved!';
      } else document.getElementById('message').textContent = 'No Solution Found';
    }
  </script>
</body>
</html>
```

## Experiment 18 — Unit Converter

**Aim:** Convert between kilometers/meters and kilograms/grams.

**File:** `experiment-18/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Unit Converter</title></head>
<body>
  <h2>Unit Converter</h2>
  Enter Value: <input type="number" id="value"><br><br>
  Select Conversion:
  <select id="type">
    <option value="km">Kilometer to Meter</option>
    <option value="m">Meter to Kilometer</option>
    <option value="kg">Kilogram to Gram</option>
    <option value="g">Gram to Kilogram</option>
  </select><br><br>
  <button onclick="convert()">Convert</button>
  <h3 id="result"></h3>
  <script>
    function convert() {
      let input = document.getElementById('value').value;
      let value = Number(input);
      let type = document.getElementById('type').value;
      if (input.trim() === '' || !Number.isFinite(value)) {
        alert('Enter a valid number'); return;
      }
      let result;
      if (type === 'km') result = value * 1000 + ' meters';
      else if (type === 'm') result = value / 1000 + ' kilometers';
      else if (type === 'kg') result = value * 1000 + ' grams';
      else result = value / 1000 + ' kilograms';
      document.getElementById('result').textContent = 'Result: ' + result;
    }
  </script>
</body>
</html>
```

## Experiment 19 — Basic Calculator

**Aim:** Perform addition, subtraction, multiplication, and division.

**File:** `experiment-19/index.html`

```html
<!DOCTYPE html>
<html>
<head><title>Calculator</title></head>
<body>
  <h2>Simple Calculator</h2>
  Number 1: <input type="number" id="n1"><br><br>
  Number 2: <input type="number" id="n2"><br><br>
  <button onclick="calculate('+')">+</button>
  <button onclick="calculate('-')">-</button>
  <button onclick="calculate('*')">*</button>
  <button onclick="calculate('/')">/</button>
  <h3 id="result"></h3>
  <script>
    function calculate(op) {
      let input1 = document.getElementById('n1').value;
      let input2 = document.getElementById('n2').value;
      if (input1.trim() === '' || input2.trim() === '') {
        alert('Enter both numbers'); return;
      }
      let a = Number(input1), b = Number(input2), result;
      if (op === '+') result = a + b;
      else if (op === '-') result = a - b;
      else if (op === '*') result = a * b;
      else {
        if (b === 0) { alert('Cannot divide by zero'); return; }
        result = a / b;
      }
      document.getElementById('result').textContent = 'Result: ' + result;
    }
  </script>
</body>
</html>
```

## Experiment 20 — Single-Page Calculator and Converter

**Aim:** Build a single-page tool that validates input and performs a selected calculation or conversion.

**File:** `experiment-20/index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Calculator and Converter</title>
  <style>
    body { font-family: Arial; text-align: center; background: lightblue; }
    .box { background: white; padding: 20px; margin: 30px auto;
           width: 350px; max-width: 85%; border-radius: 10px; }
    input, select, button { padding: 10px; margin: 5px; }
    button { background: blue; color: white; cursor: pointer; }
  </style>
</head>
<body>
  <h1>Calculator and Converter</h1>
  <div class="box">
    <h2>Enter Values</h2>
    <input type="number" id="num1" placeholder="First Number"><br>
    <input type="number" id="num2" placeholder="Second Number"><br>
    <select id="operation">
      <option value="add">Addition</option>
      <option value="sub">Subtraction</option>
      <option value="mul">Multiplication</option>
      <option value="div">Division</option>
      <option value="km">KM to Meter</option>
      <option value="kg">KG to Gram</option>
    </select><br>
    <button onclick="calculate()">Calculate</button>
    <h3 id="result"></h3>
  </div>
  <script>
    function calculate() {
      let input1 = document.getElementById('num1').value;
      let input2 = document.getElementById('num2').value;
      let op = document.getElementById('operation').value;
      if (input1.trim() === '') { alert('Enter First Number'); return; }
      if (!['km', 'kg'].includes(op) && input2.trim() === '') {
        alert('Enter Second Number'); return;
      }
      let a = Number(input1), b = Number(input2), result;
      switch (op) {
        case 'add': result = a + b; break;
        case 'sub': result = a - b; break;
        case 'mul': result = a * b; break;
        case 'div':
          if (b === 0) { alert('Division by zero not allowed'); return; }
          result = a / b; break;
        case 'km': result = a * 1000 + ' meters'; break;
        case 'kg': result = a * 1000 + ' grams'; break;
      }
      document.getElementById('result').textContent = 'Result: ' + result;
    }
  </script>
</body>
</html>
```

---

## Notes

- All examples are intended for **learning and local browser demonstrations**.
- Forms do not store submissions or connect to a database.
- The login example uses hardcoded credentials for demonstration only and is not production-safe.
- No build tools, packages, or server installation are required.

## GitHub Upload

Create a repository, add `README.md` and the experiment folders, then run:

```bash
git init
git add .
git commit -m "Add 20 web application development lab experiments"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Replace the example repository URL with your own. If your repository already has a Git remote, skip `git remote add origin`.

## Result

Twenty web development laboratory examples have been documented using HTML, CSS, and JavaScript for practice and revision.
