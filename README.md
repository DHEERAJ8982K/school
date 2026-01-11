 !<!DOCTYPE html> html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Govt Higher Secondary School Khawasa</title>
    <style>
        /* CSS Design */
        body { font-family: 'Arial', sans-serif; margin: 0; padding: 0; background-color: #f4f4f4; }
        header { background: #003366; color: white; padding: 20px; text-align: center; }
        nav { background: #004080; padding: 10px; text-align: center; sticky: top; }
        nav a { color: white; margin: 0 15px; text-decoration: none; font-weight: bold; }
        
        .container { width: 90%; margin: auto; padding: 20px; }
        h2 { text-align: center; color: #4c6885; border-bottom: 2px solid #003366; padding-bottom: 10px; }

        /* Teacher Cards */
        img-box{width: 150px;
            height: 150px;
            margin: auto 15px;
        }
        .grid { display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;
        align-items: center;
    background-color: #eee; }
        .card { background: white; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); width: 250px; padding: 15px; text-align: center; }
        .card img { width: 150px; height: 150px; border-radius: 50%; object-fit: cover; background: #ddd; }
        .card h3 { margin: 10px 0 5px; color: #333; }
        .card p { color: #666; font-size: 14px; }

        /* Lab Section */
        .lab-box { background: white; padding: 20px; margin-bottom: 20px; border-left: 5px solid #003366; display: flex; align-items: center; gap: 20px; }
        .lab-box img { width: 200px; height: 120px; border-radius: 5px; object-fit: cover; }
        
        footer { background: #333; color: white; text-align: center; padding: 15px; margin-top: 20px; }
    </style>
</head>
<body>

<header>
    <h1>GOVT. HIGHER SECONDARY SCHOOL, KHAWASA</h1>
    <p>Shiksha, Sanskar aur Safalta</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#teachers">Teachers</a>
    <a href="#labs">Labs</a>
    <a href="#contact">Contact</a>
</nav>

<div class="container" id="teachers">
    <h2>Hamare Prerna Srot (Teachers)</h2>
    <div class="grid">
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.49.03 PM.jpeg" alt="Teacher Photo"> <h3>Shri M.L.MASRAM</h3>
            <p><b>Principal</b><br>M.A.POLITICAL SCIENCE B.Ed<br>Anubhav: 20 Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 11.31.02 AM.jpeg" alt="Teacher Photo">
            <h3>Shefali bhargav</h3>
            <p><b>Vyakhyata ( MATHES)</b><br>M.Sc MATHES<br>Anubhav: 10 Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.16.42 PM (1).jpeg" alt="Teacher Photo">
            <h3>SHRI D.S.RAHANGDALE</h3>
            <p><b>Vyakhyata (Biology)</b><br>M.Sc Botany<br>Anubhav: 8 Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.06.11 PM.jpeg" alt="Teacher Photo">
            <h4>SHRI PRAKASH THOTEY</h4>
            <p><b>Vyakhyata (MATHES)</b><br>M.Sc MATHES<br>Anubhav: 20 Varsh</p>
        </div>
        <div class="card">
            <img src="teacher3.jpg" alt="Teacher Photo">
            <h5>SHRI VEER NARAYAN TEKAM</h5>
            <p><b>Vyakhyata (ENGLISH)</b><br>M.Sc ENGLISH<br>Anubhav: 16 Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.33.53 PM.jpeg" alt="Teacher Photo">
            <h6>SHRI M.L.MARSKOLE</h6>
            <p><b>Vyakhyata (HINDI)</b><br>M.Sc HINDI<br>Anubhav: 23 Varsh</p>
        </div>
        <div class="card">
            <img src=" c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.29.16 PM.jpeg" alt="Teacher Photo">
            <h5>SMT.REKHA DAHERWAL</h5>
            <p><b>(SCIENCE)</b><br>M.Sc SCIENCE<br>Anubhav: 8 Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.07.25 PM.jpeg" alt="Teacher Photo">
            <h5>DHEERAJ 
            KUMAR SHRIVAS</h5>
            <p><b>VOCATIONAL TRAINER (INFORMATION TECHNOLOGY)</b><br>B.TECH IT<br>Anubhav: 6 Varsh</p>
        </div>
        <div class="card">
            <div><style></style></div>
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.47.24 PM.jpeg" alt="Teacher Photo">
            <h6>MAYANK RAJ WASNIK</h6>
            <p><b>VOCATIONAL TRAINER(E.T)</b><br>M.E.ELECTRONICS<br>Anubhav: 9Varsh</p>
        </div>
        <div class="card">
            <img src="c:\Users\dheeraj shrivas\Downloads\WhatsApp Image 2026-01-11 at 12.51.50 PM.jpeg" alt="Teacher Photo">
            <h4>11TH IT KE STUDENTS</h4>
            <p><b> 11TH</b>
        </div>
    </div>
</div>

<div class="container" id="labs">
    <h2>Vigyan Prayogshala (Our Labs)</h2>
    
    <div class="lab-box">
        <img src="physics-lab.jpg" alt="Physics Lab">
        <div>
            <h3>Physics Lab</h3>
            <p>Hamari Physics lab modern upkarno se lais hai jahan bacche optics, electricity aur mechanics ke prayog karte hain.</p>
        </div>
    </div>

    <div class="lab-box">
        <img src="chemistry-lab.jpg" alt="Chemistry Lab">
        <div>
            <h3>Chemistry Lab</h3>
            <p>Surakshit vatavaran mein rasayanik prayogo ke liye uchit vyavastha aur chemicals uplabdha hain.</p>
        </div>
    </div>

    <div class="lab-box">
        <img src="computer-lab.jpg" alt="Computer Lab">
        <div>
            <h3>Computer Lab</h3>
            <p>Internet suvidha ke sath 20 se zyada computers bacchon ko digital shiksha pradan karte hain.</p>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2026 GHSS Khawasa | Developed for School Excellence</p>
</footer>

</body>
</html>
