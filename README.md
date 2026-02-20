# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Interactive Player Stats Table - Blackburn vs Preston Defensive Stats</title>
  <style>
    body { font-family: Arial, sans-serif; }
    table {
      border-collapse: collapse;
      width: 100%;
      margin: 20px 0;
    }
    th, td {
      border: 1px solid #ddd;
      padding: 8px;
      text-align: center;
    }
    th {
      background-color: #f2f2f2;
    }
    /* Highlight classes */
    .highlight-col {
      background-color: #fffacd !important; /* light yellow for columns */
    }
    .highlight-row {
      background-color: #e6f3ff !important; /* light blue for rows/players */
    }
    /* Controls */
    .toggles {
      margin: 15px 0;
      font-size: 0.95em;
    }
    .toggles label {
      margin-right: 15px;
      cursor: pointer;
      display: inline-block;
      margin-bottom: 8px;
    }
    .player-toggles {
      margin-top: 20px;
    }
  </style>
</head>
<body>

<h2>Blackburn Rovers vs Preston North End - Player Defensive Stats (researched data)</h2>

<!-- Column highlight toggles -->
<div class="toggles">
  <strong>Highlight columns:</strong><br>
  <label><input type="checkbox" data-col="2"> Fouls Committed p90</label>
  <label><input type="checkbox" data-col="3"> Fouls Won p90</label>
  <label><input type="checkbox" data-col="4"> Tackles p90</label>
  <label><input type="checkbox" data-col="5"> YC (tot)</label>
  <label><input type="checkbox" data-col="6"> RC (tot)</label>
</div>

<!-- Player (row) highlight toggles -->
<div class="toggles player-toggles">
  <strong>Highlight players (rows):</strong><br>
  <label><input type="checkbox" data-player="Balazs Toth"> Balazs Toth</label>
  <label><input type="checkbox" data-player="Sean McLoughlin"> Sean McLoughlin</label>
  <label><input type="checkbox" data-player="Hayden Carter"> Hayden Carter</label>
  <label><input type="checkbox" data-player="Eiran Cashin"> Eiran Cashin</label>
  <label><input type="checkbox" data-player="Ryan Alebiosu"> Ryan Alebiosu</label>
  <label><input type="checkbox" data-player="Sondre Tronstad"> Sondre Tronstad</label>
  <label><input type="checkbox" data-player="Moussa Baradji"> Moussa Baradji</label>
  <label><input type="checkbox" data-player="Harry Pickering"> Harry Pickering</label>
  <label><input type="checkbox" data-player="Ryoya Morishita"> Ryoya Morishita</label>
  <label><input type="checkbox" data-player="Mathias Jørgensen"> Mathias Jørgensen</label>
  <label><input type="checkbox" data-player="Andri Gudjohnsen"> Andri Gudjohnsen</label>
  <label><input type="checkbox" data-player="David Cornell"> David Cornell</label>
  <label><input type="checkbox" data-player="Andrew Hughes"> Andrew Hughes</label>
  <label><input type="checkbox" data-player="Jordan Storey"> Jordan Storey</label>
  <label><input type="checkbox" data-player="Lewis Gibson"> Lewis Gibson</label>
  <label><input type="checkbox" data-player="Andrija Vukcevic"> Andrija Vukcevic</label>
  <label><input type="checkbox" data-player="Pol Valentin"> Pol Valentin</label>
  <label><input type="checkbox" data-player="Alistair McCann"> Alistair McCann</label>
  <label><input type="checkbox" data-player="Ben Whiteman"> Ben Whiteman</label>
  <label><input type="checkbox" data-player="Alfie Devine"> Alfie Devine</label>
  <label><input type="checkbox" data-player="Lewis Dobbin"> Lewis Dobbin</label>
  <label><input type="checkbox" data-player="Milutin Osmajic"> Milutin Osmajic</label>
</div>

<table id="statsTable">
  <thead>
    <tr>
      <th>Player</th>
      <th>Fouls Committed p90</th>
      <th>Fouls Won p90</th>
      <th>Tackles p90</th>
      <th>YC (tot)</th>
      <th>RC (tot)</th>
    </tr>
  </thead>
  <tbody>
    <tr data-player-name="Balazs Toth">
      <td>Balazs Toth</td>
      <td>0.00</td>
      <td>0.00</td>
      <td>0.00</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Sean McLoughlin">
      <td>Sean McLoughlin</td>
      <td>0.58</td>
      <td>0.58</td>
      <td>1.60</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr data-player-name="Hayden Carter">
      <td>Hayden Carter</td>
      <td>0.88</td>
      <td>0.00</td>
      <td>0.88</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Eiran Cashin">
      <td>Eiran Cashin</td>
      <td>0.94</td>
      <td>0.28</td>
      <td>4.05</td>
      <td>3</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Ryan Alebiosu">
      <td>Ryan Alebiosu</td>
      <td>0.68</td>
      <td>0.23</td>
      <td>2.11</td>
      <td>3</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Sondre Tronstad">
      <td>Sondre Tronstad</td>
      <td>0.96</td>
      <td>0.72</td>
      <td>2.64</td>
      <td>8</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Moussa Baradji">
      <td>Moussa Baradji</td>
      <td>2.28</td>
      <td>1.59</td>
      <td>3.08</td>
      <td>3</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Harry Pickering">
      <td>Harry Pickering</td>
      <td>1.17</td>
      <td>0.88</td>
      <td>0.29</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Ryoya Morishita">
      <td>Ryoya Morishita</td>
      <td>1.23</td>
      <td>1.29</td>
      <td>1.23</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Mathias Jørgensen">
      <td>Mathias Jørgensen</td>
      <td>0.00</td>
      <td>0.19</td>
      <td>0.19</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Andri Gudjohnsen">
      <td>Andri Gudjohnsen</td>
      <td>1.25</td>
      <td>1.38</td>
      <td>0.26</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr data-player-name="David Cornell">
      <td>David Cornell</td>
      <td>0.00</td>
      <td>0.00</td>
      <td>0.00</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Andrew Hughes">
      <td>Andrew Hughes</td>
      <td>1.26</td>
      <td>0.55</td>
      <td>1.63</td>
      <td>8</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Jordan Storey">
      <td>Jordan Storey</td>
      <td>0.69</td>
      <td>0.92</td>
      <td>1.32</td>
      <td>6</td>
      <td>1</td>
    </tr>
    <tr data-player-name="Lewis Gibson">
      <td>Lewis Gibson</td>
      <td>0.58</td>
      <td>1.15</td>
      <td>1.21</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Andrija Vukcevic">
      <td>Andrija Vukcevic</td>
      <td>1.57</td>
      <td>0.14</td>
      <td>1.43</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Pol Valentin">
      <td>Pol Valentin</td>
      <td>1.10</td>
      <td>1.23</td>
      <td>3.29</td>
      <td>2</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Alistair McCann">
      <td>Alistair McCann</td>
      <td>1.68</td>
      <td>0.81</td>
      <td>4.17</td>
      <td>4</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Ben Whiteman">
      <td>Ben Whiteman</td>
      <td>1.21</td>
      <td>0.29</td>
      <td>1.90</td>
      <td>8</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Alfie Devine">
      <td>Alfie Devine</td>
      <td>0.72</td>
      <td>0.81</td>
      <td>1.70</td>
      <td>3</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Lewis Dobbin">
      <td>Lewis Dobbin</td>
      <td>0.66</td>
      <td>1.08</td>
      <td>0.78</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr data-player-name="Milutin Osmajic">
      <td>Milutin Osmajic</td>
      <td>0.90</td>
      <td>1.39</td>
      <td>0.65</td>
      <td>3</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

<script>
  // Column highlighting
  document.querySelectorAll('.toggles input[data-col]').forEach(checkbox => {
    checkbox.addEventListener('change', function() {
      const colIndex = parseInt(this.getAttribute('data-col'));
      const table = document.getElementById('statsTable');
      const cells = table.querySelectorAll(`td:nth-child(${colIndex}), th:nth-child(${colIndex})`);
      cells.forEach(cell => {
        if (this.checked) {
          cell.classList.add('highlight-col');
        } else {
          cell.classList.remove('highlight-col');
        }
      });
    });
  });

  // Player row highlighting
  document.querySelectorAll('.player-toggles input[data-player]').forEach(checkbox => {
    checkbox.addEventListener('change', function() {
      const playerName = this.getAttribute('data-player');
      const rows = document.querySelectorAll(`tr[data-player-name="${playerName}"]`);
      rows.forEach(row => {
        if (this.checked) {
          row.classList.add('highlight-row');
        } else {
          row.classList.remove('highlight-row');
        }
      });
    });
  });
</script>

</body>
</html>