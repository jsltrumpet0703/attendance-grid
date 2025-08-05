<!DOCTYPE html>
<html>
<head>
  <title>Attendance Grid with Names and Days</title>
  <style>
    body { font-family: sans-serif; padding: 20px; }
    .grid-container {
      display: grid;
      grid-template-columns: 80px repeat(5, 60px);
      gap: 10px;
      align-items: center;
    }
    .header {
      font-weight: bold;
      text-align: center;
    }
    .name-cell {
      font-weight: bold;
      text-align: right;
      padding-right: 10px;
    }
    .cell {
      width: 60px;
      height: 60px;
      background-color: lightgray;
      border: 1px solid #ccc;
      cursor: pointer;
      border-radius: 6px;
    }
  </style>
</head>
<body>
  <h2>Class Attendance Tracker</h2>
  <div class="grid-container" id="grid">
    <div></div>
    <div class="header">Day 1</div>
    <div class="header">Day 2</div>
    <div class="header">Day 3</div>
    <div class="header">Day 4</div>
    <div class="header">Day 5</div>
    <div class="name-cell">A</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">B</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">C</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">D</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">E</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">F</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">G</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
    <div class="name-cell">H</div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div><div class="cell" data-state="0"></div>
  </div>
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const colors = ["lightgray", "green", "yellow", "red"];
      const cells = document.querySelectorAll(".cell");
      cells.forEach(cell => {
        cell.addEventListener("click", () => {
          let state = parseInt(cell.getAttribute("data-state")) || 0;
          state = (state + 1) % colors.length;
          cell.setAttribute("data-state", state);
          cell.style.backgroundColor = colors[state];
        });
        let state = parseInt(cell.getAttribute("data-state")) || 0;
        cell.style.backgroundColor = colors[state];
      });
    });
  </script>
</body>
</html>
