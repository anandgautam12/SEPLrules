
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SEPL – Official Rules & Guidelines</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
/* Reset & Global */
* { margin: 0; padding: 0; box-sizing: border-box; scroll-behavior: smooth; }
body { font-family: 'Poppins', sans-serif; background: #0f2027; color: #fff; }

/* Layout */
.container { display: flex; min-height: 100vh; }
.sidebar {
    position: sticky;
    top: 0;
    width: 260px;
    background: #1c1c1c;
    padding: 20px;
    flex-shrink: 0;
    border-right: 1px solid #333;
}
.sidebar h2 { font-size: 22px; font-weight: 700; margin-bottom: 20px; text-align:center; }
.sidebar button {
    width: 100%;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    border-radius: 10px;
    background: #292929;
    color: #fff;
    font-weight: 600;
    font-size: 16px;
    text-align: left;
    cursor: pointer;
    display: flex;
    align-items: center;
    transition: 0.3s;
}
.sidebar button i { margin-right: 12px; color: #ffd700; }
.sidebar button:hover, .sidebar button.active { background: linear-gradient(135deg,#ff4e50,#f9d423); color:#000; }

/* Main Content */
.main-content {
    flex: 1;
    padding: 30px;
}
.content-card {
    background: rgba(255,255,255,0.05);
    border-radius: 15px;
    padding: 25px;
    margin-bottom: 20px;
    display: none;
    animation: fadeIn 0.5s ease forwards;
}
.content-card h3 { font-size: 22px; color: #ffd700; margin-bottom: 15px; }

/* Table */
table {
    width: 100%;
    border-collapse: collapse;
    border-radius: 10px;
    overflow: hidden;
    margin-top: 10px;
}
th, td {
    padding: 12px;
    border: 1px solid #ffffff33;
    text-align: center;
    font-size: 16px;
}
th { background: linear-gradient(135deg,#ff4e50,#f9d423); color: #fff; }
td { background: rgba(255,255,255,0.05); }

/* Animations */
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
}

/* Header */
.header {
    text-align: center;
    padding: 30px 20px;
    background: linear-gradient(135deg,#1e3c72,#2a5298);
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.4);
    margin-bottom: 20px;
}
.header img {
    width: 150px;
    border-radius: 50%;
    border: 3px solid #fff;
    margin-bottom: 15px;
}
.header h1 { font-size: 36px; font-weight: 700; text-shadow: 2px 2px 8px rgba(0,0,0,0.5); }
.header h2 { font-size: 20px; font-weight: 500; color: #f5f5f5; text-shadow: 1px 1px 4px rgba(0,0,0,0.4); }

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: #111;
    font-size: 14px;
    color: #888;
    margin-top: 20px;
}
</style>
</head>
<body>

<div class="header">
    <img src="mainlogo.jpg" alt="SEPL Logo">
    <h1>SEPL – Satpuda Engineering Premier League</h1>
    <h2>Season 01 – Official Rules & Guidelines</h2>
</div>

<div class="container">
    <!-- Sidebar -->
    <div class="sidebar">
        <h2>Rules Navigation</h2>
        <button onclick="showRule(1)" id="btn1"><i class="fas fa-user-plus"></i> Registration Rules</button>
        <button onclick="showRule(2)" id="btn2"><i class="fas fa-users"></i> Team Squad Rules</button>
        <button onclick="showRule(3)" id="btn3"><i class="fas fa-star"></i> Icon Player Rule</button>
        <button onclick="showRule(4)" id="btn4"><i class="fas fa-shield-alt"></i> Playing XI Composition</button>
        <button onclick="showRule(5)" id="btn5"><i class="fas fa-file-alt"></i> Match Sheet</button>
        <button onclick="showRule(6)" id="btn6"><i class="fas fa-table"></i> League Format</button>
        <button onclick="showRule(7)" id="btn7"><i class="fas fa-gavel"></i> Auction Rules</button>
        <button onclick="showRule(8)" id="btn8"><i class="fas fa-cricket"></i> Match Rules </button>
        <button onclick="showRule(9)" id="btn9"><i class="fas fa-running"></i> Trials Rules</button>
    </div>

    <!-- Main Content -->
    <div class="main-content">
        <div class="content-card" id="rule1">
            <h3>Player & Team Registration Fees</h3>
            <p>• Player Registration Fee: ₹200 <br>• Team Owner Registration Fee: ₹3000</p>
        </div>

        <div class="content-card" id="rule2">
            <h3>Squad Composition</h3>
            <p>• Minimum Squad Size: 14 players <br>• Maximum Squad Size: 16 players <br>• Faculty Players in Squad: Max 5 <br>• Faculty in Playing XI: Max 2 &Squad</p>
        </div>

        <div class="content-card" id="rule3">
            <h3>Icon Player</h3>
            <p>Every team must have 1 Faculty Icon Player. <p>The Icon Player guides the team during the auction process.</p>
        </div>

        <div class="content-card" id="rule4">
            <h3>Playing XI Composition</h3>
            <p>• Faculty:Minimum 1 <br>• Final/3rd Year/Polytechnic:Minimum 2 <br>• 2nd Year:Minimum 2 <br>• 1st Year:Minimum 2 <br>• ITI: Minimum2</p>
        </div>

        <div class="content-card" id="rule5">
            <h3>Match Sheet</h3>
            <table>
                <tr>
                    <th>Sr No.</th>
                    <th>Player Name</th>
                    <th>Role</th>
                    <th>Year</th>
                    <th>Branch</th>
                    <th>Roll No.</th>
                    <th>Coach Verify</th>
                    <th>Captain Sign</th>
                </tr>
                <tr><td>1</td><td>---</td><td>---</td><td>---</td><td>---</td><td>---</td><td>---</td><td>---</td></tr>
            </table>
        </div>

        <div class="content-card" id="rule6">
            <h3>League Structure</h3>
            <p>• The league will consist of a total of 32 matches.



 <br>•The Table Topper (1st place) will qualify directly for the Final.<br>• The teams in 2nd and 3rd position will play a Qualifier match. <br>• The Winner of the Qualifier and the Table Topper will play in the Grand Final.
</p>
        </div>

        <div class="content-card" id="rule7">
            <h3>Auction Details</h3>
            <p>• Base Price: ₹300 <br>• ₹300–700: +₹50 increment <br>• Above ₹700: +₹100 increment <br>• Unsold Players → Re-auction</p>
        </div>

        <div class="content-card" id="rule8">
            <h3>Match Rules </h3>
            <p>• Match Duration: 8 Overs per side <br>
               • Max 2 Overs per Bowler <br>
               • Bowling: Overarm only <br>
               • Powerplay: Total of 3 overs.

             <p> The first 2 overs are compulsory powerplay.

              <p> batting team can choose 1 over of powerplay between the 6th and 8th over.

<br>
               • Free Hit: After No-ball <br>
               • No Leg Byes / LBW applies per umpire discretion <br>
               • DRS not available <br>
               • Umpire Decision is Final</p>
        </div>

        <div class="content-card" id="rule9">
            <h3>Trial Match Rules</h3>
            <p>• Batsman: 2 Overs <br>• Bowler: 2 Overs <br>• All-rounder: 1 Over Bat + 1 Over Bowl</p>
        </div>
    </div>
</div>

<footer>
    &copy; 2025 SEPL. All Rights Reserved.
</footer>

<script>
function showRule(id) {
    // Hide all cards
    const cards = document.querySelectorAll('.content-card');
    cards.forEach(card => card.style.display = 'none');

    // Remove active from all buttons
    const buttons = document.querySelectorAll('.sidebar button');
    buttons.forEach(btn => btn.classList.remove('active'));

    // Show selected card
    document.getElementById('rule' + id).style.display = 'block';
    document.getElementById('btn' + id).classList.add('active');
}

// Show first rule by default
showRule(1);
</script>

</body>
</html>

