# stake-ui
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Stake UI Demo</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <header class="topbar">
    <div class="logo">Stake</div>
    <div class="actions">
      <button class="btn">Login</button>
      <button class="btn primary">Register</button>
    </div>
  </header>

  <div class="layout">
    <aside class="sidebar">
      <h3>Casino</h3>
      <ul>
        <li>Mines</li>
        <li>Plinko</li>
        <li>Sweet Bonanza</li>
        <li>Crash</li>
      </ul>
    </aside>

    <main class="content">
      <h2>Popular Games</h2>
      <div class="games">
        <div class="card">Sweet Bonanza</div>
        <div class="card">Mines</div>
        <div class="card">Plinko</div>
        <div class="card">Crash</div>
        <div class="card">Dice</div>
        <div class="card">Roulette</div>
      </div>
    </main>
  </div>

</body>
</html>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0b1220;
  color: #fff;
}

/* Top Bar */
.topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  background: #020617;
  border-bottom: 1px solid #1e293b;
}

.logo {
  font-size: 22px;
  font-weight: bold;
  color: #22c55e;
}

.actions .btn {
  background: transparent;
  border: 1px solid #334155;
  color: white;
  padding: 8px 15px;
  margin-left: 10px;
  border-radius: 6px;
  cursor: pointer;
}

.actions .primary {
  background: #22c55e;
  color: black;
  border: none;
}

/* Layout */
.layout {
  display: flex;
}

/* Sidebar */
.sidebar {
  width: 220px;
  background: #020617;
  min-height: calc(100vh - 60px);
  padding: 20px;
}

.sidebar h3 {
  margin-top: 0;
  color: #38bdf8;
}

.sidebar ul {
  padding: 0;
}

.sidebar li {
  list-style: none;
  margin: 15px 0;
  cursor: pointer;
  color: #cbd5f5;
}

.sidebar li:hover {
  color: #22c55e;
}

/* Content */
.content {
  flex: 1;
  padding: 25px;
}

.games {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 20px;
}

.card {
  background: #1e293b;
  height: 120px;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  transition: 0.2s;
}

.card:hover {
  transform: scale(1.05);
  background: #334155;
}
