<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TFA - World Cup Of Aerobics</title>
    <style>
        body { background-color: #1a1a1a; color: white; font-family: 'Segoe UI', sans-serif; text-align: center; margin: 0; padding-bottom: 50px; }
        .header { background: linear-gradient(135deg, #4b0082, #000); padding: 40px 20px; border-bottom: 4px solid #FFD700; }
        h1 { color: #FFD700; margin: 0; font-size: 32px; text-transform: uppercase; }
        .slogan { color: #fff; font-style: italic; font-size: 18px; letter-spacing: 2px; margin-top: 5px; }
        .event-theme { background: #FFD700; color: #000; padding: 10px; font-weight: bold; font-size: 20px; margin-top: 20px; display: inline-block; border-radius: 5px; }
        
        /* Grid for 30 Instructors */
        .instructor-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); 
            gap: 20px; 
            padding: 20px; 
            max-width: 1200px; 
            margin: 0 auto;
        }
        .bio-card { 
            background: #2d2d2d; 
            border-radius: 15px; 
            overflow: hidden; 
            border: 1px solid #444;
            transition: transform 0.3s;
        }
        .bio-card:hover { transform: translateY(-5px); border-color: #FFD700; }
        .photo-placeholder { 
            width: 100%; 
            height: 200px; 
            background: #444; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            color: #888;
            font-size: 14px;
        }
        .bio-info { padding: 15px; text-align: left; }
        .bio-name { color: #FFD700; font-weight: bold; font-size: 18px; margin-bottom: 5px; }
        .bio-text { font-size: 14px; color: #ccc; line-height: 1.4; }

        .footer-whatsapp { background: #25D366; color: white; padding: 15px; position: fixed; bottom: 20px; right: 20px; border-radius: 50px; text-decoration: none; font-weight: bold; box-shadow: 0 4px 10px rgba(0,0,0,0.3); }
    </style>
</head>
<body>

<div class="header">
    <h1>TOTAL FITNESS ACADEMY (TFA)</h1>
    <div class="slogan">"Eyomphakathi"</div>
    <div class="event-theme">🏆 THEME: WORLD CUP OF AEROBICS 🏆</div>
</div>

<div style="margin-top: 40px;">
    <h2 style="color: #FFD700;">MEET THE 30 LEAD INSTRUCTORS</h2>
    <p>Loading the elite team for the annual event...</p>
</div>

<div class="instructor-grid">
    <div class="bio-card">
        <div class="photo-placeholder">PHOTO SPACE</div>
        <div class="bio-info">
            <div class="bio-name">INSTRUCTOR: CBONZA</div>
            <div class="bio-text">Branch: Between Midway Crossing & KwaMashu Station. Professional lead instructor at TFA.</div>
        </div>
    </div>

    <div class="bio-card">
        <div class="photo-placeholder">PHOTO SPACE</div>
        <div class="bio-info">
            <div class="bio-name">INSTRUCTOR: LUNGISA</div>
            <div class="bio-text">Branch: Near Bridge City Shopping Centre. Expert in high-intensity aerobics.</div>
        </div>
    </div>

    <div class="bio-card">
        <div class="photo-placeholder">PHOTO SPACE</div>
        <div class="bio-info">
            <div class="bio-name">INSTRUCTOR: LINDA</div>
            <div class="bio-text">Branch: Near Midway Crossing Mall. Specializing in rhythm and endurance.</div>
        </div>
    </div>

    <script>
        const grid = document.querySelector('.instructor-grid');
        for (let i = 4; i <= 30; i++) {
            grid.innerHTML += `
                <div class="bio-card">
                    <div class="photo-placeholder">PHOTO SPACE</div>
                    <div class="bio-info">
                        <div class="bio-name">INSTRUCTOR ${i}: [NAME]</div>
                        <div class="bio-text">Bio and achievement details for the World Cup of Aerobics will be added here.</div>
                    </div>
                </div>`;
        }
    </script>
</div>

<a href="https://wa.me/27XXXXXXXXX" class="footer-whatsapp">Register via WhatsApp</a>

</body>
</html>
