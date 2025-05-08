<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Northern Europe Winter Adventure</title>
  <style>
    :root {
      --primary: #2c3e50;
      --secondary: #2980b9;
      --light: #f0f4f8;
      --white: #ffffff;
      --shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      background: var(--light);
      color: #333;
      margin: 0;
      padding: 0;
    }
    
    header {
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      color: white;
      padding: 2rem 0;
      text-align: center;
      margin-bottom: 2rem;
    }
    
    h1, h2, h3 {
      color: var(--primary);
      margin-top: 0;
    }
    
    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    
    .subtitle {
      font-size: 1.2rem;
      opacity: 0.9;
    }
    
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 20px;
    }
    
    nav {
      background: var(--white);
      padding: 1rem;
      box-shadow: var(--shadow);
      position: sticky;
      top: 0;
      z-index: 100;
    }
    
    nav ul {
      display: flex;
      justify-content: center;
      list-style: none;
      padding: 0;
      margin: 0;
      flex-wrap: wrap;
    }
    
    nav li {
      margin: 0 15px;
    }
    
    nav a {
      color: var(--primary);
      text-decoration: none;
      font-weight: 600;
      padding: 5px 0;
      border-bottom: 2px solid transparent;
      transition: all 0.3s ease;
    }
    
    nav a:hover, nav a.active {
      color: var(--secondary);
      border-bottom-color: var(--secondary);
    }
    
    .section {
      background: var(--white);
      padding: 2rem;
      border-radius: 8px;
      box-shadow: var(--shadow);
      margin-bottom: 2rem;
    }
    
    .print-button {
      background: #2980b9;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      margin: 20px 0;
      display: inline-block;
    }
    
    .summary-table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
    }
    
    .summary-table th, .summary-table td {
      border: 1px solid #ddd;
      padding: 8px;
      text-align: left;
    }
    
    .summary-table th {
      background-color: #f2f2f2;
    }
    
    .transport-icon {
      width: 20px;
      height: 20px;
      vertical-align: middle;
      margin-right: 5px;
    }
    
    .itinerary-day {
      border-left: 4px solid var(--secondary);
      padding-left: 1.5rem;
      margin-bottom: 2rem;
    }
    
    .day-title {
      display: flex;
      align-items: center;
      margin-bottom: 1rem;
    }
    
    .day-number {
      background: var(--secondary);
      color: white;
      width: 40px;
      height: 40px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 1rem;
      font-weight: bold;
    }
    
    .action-item {
      background: #fff8e1;
      border-left: 4px solid #ffc107;
      padding: 1rem;
      margin: 1rem 0;
    }
    
    .action-title {
      font-weight: bold;
      color: #ff9800;
      margin-bottom: 0.5rem;
    }
    
    footer {
      background: var(--primary);
      color: white;
      text-align: center;
      padding: 2rem 0;
      margin-top: 3rem;
    }
    
    @media (max-width: 768px) {
      nav ul {
        flex-direction: column;
        align-items: center;
      }
      
      nav li {
        margin: 5px 0;
      }
      
      .summary-table {
        font-size: 14px;
      }
    }
    
    @media print {
      @page { size: A4; margin: 1cm; }
      body { font-size: 12pt; background: white; }
      nav, footer { display: none; }
      .section { break-inside: avoid; }
      .print-button { display: none; }
    }
  </style>
</head>
<body>
  <header>
    <div class="container">
      <h1>Northern Europe Winter Adventure</h1>
      <p class="subtitle">Denmark • Iceland • Finland | December 20 - January 3</p>
    </div>
  </header>

  <nav>
    <div class="container">
      <ul>
        <li><a href="#summary" class="active">Summary</a></li>
        <li><a href="#itinerary">Itinerary</a></li>
        <li><a href="#logistics">Logistics</a></li>
        <li><a href="#gallery">Gallery</a></li>
      </ul>
    </div>
  </nav>

  <div class="container">
    <section id="summary" class="section">
      <h2>⏱️ Trip Summary</h2>
      <button class="print-button" onclick="window.print()">Download Printable PDF</button>
      
      <table class="summary-table">
        <tr>
          <th>Route</th>
          <th>Date</th>
          <th>Mode</th>
          <th>Action Required</th>
        </tr>
        <tr>
          <td>Home → Copenhagen</td>
          <td>20 Dec (arrive 13:15)</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight</td>
          <td>Book arrival (CPH)</td>
        </tr>
        <tr>
          <td>Copenhagen → Reykjavík</td>
          <td>23 Dec (depart night)</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight</td>
          <td>Compare <a href="https://www.flysas.com/" target="_blank">SAS</a>/<a href="https://www.icelandair.com/" target="_blank">Icelandair</a></td>
        </tr>
        <tr>
          <td>Reykjavík → Rovaniemi</td>
          <td>28 Dec (depart night)</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight</td>
          <td>Or overnight in HEL</td>
        </tr>
        <tr>
          <td>Rovaniemi → Helsinki</td>
          <td>30 Dec</td>
          <td>
            <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight or 
            <img src="https://cdn-icons-png.flaticon.com/512/619/619165.png" class="transport-icon" alt="Train"> Train
          </td>
          <td>Choose preferred mode</td>
        </tr>
        <tr>
          <td>Helsinki ↔ Tallinn</td>
          <td>1 Jan</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/2061/2061118.png" class="transport-icon" alt="Ferry"> Ferry</td>
          <td>Reserve via <a href="https://www.tallinksilja.com/" target="_blank">Tallink Silja</a></td>
        </tr>
        <tr>
          <td>Helsinki → Copenhagen</td>
          <td>2 Jan</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight</td>
          <td>-</td>
        </tr>
        <tr>
          <td>Copenhagen → Home</td>
          <td>3 Jan</td>
          <td><img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"> Flight</td>
          <td>Book return from HEL</td>
        </tr>
      </table>
    </section>

    <section id="itinerary" class="section">
      <h2>🗓️ Detailed Day-by-Day Itinerary</h2>
      
      <h3>🇩🇰 Denmark (Dec 20-23)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">1</div>
          <h4>Dec 20: Arrival in Copenhagen <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"></h4>
        </div>
        <ul>
          <li><strong>13:15:</strong> Flight arrives at CPH</li>
          <li><strong>Afternoon:</strong> <a href="https://www.visitcopenhagen.com/copenhagen/nyhavn-gdk410881" target="_blank">Nyhavn harbor</a> walk</li>
          <li><strong>Evening:</strong> <a href="https://www.tivoli.dk/en/" target="_blank">Tivoli Gardens</a> Christmas market</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">2</div>
          <h4>Dec 21: LEGOLAND Adventure <img src="https://cdn-icons-png.flaticon.com/512/619/619165.png" class="transport-icon" alt="Train"></h4>
        </div>
        <ul>
          <li><strong>08:00:</strong> Train to Billund (3h)</li>
          <li><strong>All day:</strong> <a href="https://www.legoland.dk/en/" target="_blank">LEGOLAND Billund</a></li>
          <li><strong>18:00:</strong> Return to Copenhagen</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">3</div>
          <h4>Dec 22: Copenhagen Free Day</h4>
        </div>
        <ul>
          <li><strong>Options:</strong></li>
          <li>- <a href="https://www.kongernessamling.dk/en/rosenborg/" target="_blank">Rosenborg Castle</a> & hot chocolate</li>
          <li>- Day trip to <a href="https://www.malmotown.com/" target="_blank">Malmö, Sweden</a></li>
          <li>- <a href="https://www.visitcopenhagen.com/copenhagen/shopping/stroget-gdk586951" target="_blank">Strøget shopping street</a></li>
        </ul>
      </div>

      <h3>🇮🇸 Iceland (Dec 23-28)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">4</div>
          <h4>Dec 23: Fly to Reykjavík <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"></h4>
        </div>
        <ul>
          <li><strong>21:00:</strong> Night flight to KEF</li>
          <li><strong>Evening:</strong> <a href="https://www.hallgrimskirkja.is/" target="_blank">Hallgrímskirkja</a> + Christmas market</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">5</div>
          <h4>Dec 24: Golden Circle (Christmas Eve)</h4>
        </div>
        <ul>
          <li><a href="https://www.thingvellir.is/en" target="_blank">Þingvellir National Park</a></li>
          <li><a href="https://www.inspiredbyiceland.com/place/geysir/" target="_blank">Geysir</a> hot springs</li>
          <li><a href="https://www.gullfoss.is/" target="_blank">Gullfoss waterfall</a></li>
          <li><strong>Evening:</strong> Traditional Christmas dinner</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">6</div>
          <h4>Dec 25: Christmas Relaxation</h4>
        </div>
        <ul>
          <li><strong>Afternoon:</strong> <a href="https://www.bluelagoon.com/" target="_blank">Blue Lagoon</a> or <a href="https://sky.is/" target="_blank">Sky Lagoon</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">7</div>
          <h4>Dec 26: South Coast Adventure</h4>
        </div>
        <ul>
          <li><a href="https://www.south.is/en/place/seljalandsfoss" target="_blank">Seljalandsfoss</a> waterfall</li>
          <li><a href="https://www.skogafoss.is/" target="_blank">Skógafoss</a> waterfall</li>
          <li><a href="https://www.visitreykjanes.is/en/reynisfjara" target="_blank">Reynisfjara black sand beach</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">8</div>
          <h4>Dec 27: Optional Activities</h4>
        </div>
        <ul>
          <li><a href="https://www.west.is/en/service/traveling-in-snaefellsnes" target="_blank">Snæfellsnes Peninsula</a> (Kirkjufell mountain)</li>
          <li>OR <a href="https://guidetoiceland.is/book-tours-holiday/northern-lights-tours" target="_blank">Northern Lights tour</a></li>
        </ul>
      </div>

      <h3>🇫🇮 Finland (Dec 28 - Jan 3)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">9</div>
          <h4>Dec 28: Fly to Rovaniemi <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"></h4>
        </div>
        <ul>
          <li><strong>Afternoon:</strong> <a href="https://santaclausvillage.info/" target="_blank">Santa Claus Village</a></li>
          <li><strong>Evening:</strong> Arctic Circle ceremony</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">10</div>
          <h4>Dec 29: Rovaniemi Activities</h4>
        </div>
        <ul>
          <li><a href="https://www.visitrovaniemi.fi/see-and-do/safaris-and-activities/husky-safaris/" target="_blank">Husky sledding</a></li>
          <li><a href="https://wildaboutlapland.com/snowmobile-tours-rovaniemi/" target="_blank">Snowmobile safari</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">11</div>
          <h4>Dec 30: Travel to Levi <img src="https://cdn-icons-png.flaticon.com/512/619/619165.png" class="transport-icon" alt="Train"></h4>
        </div>
        <ul>
          <li><strong>Afternoon:</strong> Check-in at <a href="https://www.levi.fi/en" target="_blank">Levi ski resort</a></li>
          <li><strong>Evening:</strong> Northern Lights hunting</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">12</div>
          <h4>Dec 31: New Year's Eve in Levi</h4>
        </div>
        <ul>
          <li><a href="https://www.levi.fi/en/skiing" target="_blank">Skiing/snowboarding</a></li>
          <li>NYE fireworks</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">13</div>
          <h4>Jan 1: Tallinn Day Trip <img src="https://cdn-icons-png.flaticon.com/512/2061/2061118.png" class="transport-icon" alt="Ferry"></h4>
        </div>
        <ul>
          <li><a href="https://www.tallink.com/" target="_blank">Ferry to Tallinn</a></li>
          <li><a href="https://www.oldehansa.ee/" target="_blank">Medieval dinner at Olde Hansa</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">14</div>
          <h4>Jan 2: Helsinki Exploration <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"></h4>
        </div>
        <ul>
          <li><a href="https://www.suomenlinna.fi/en/" target="_blank">Suomenlinna Fortress</a></li>
          <li><a href="https://www.loylyhelsinki.fi/en/" target="_blank">Löyly sauna</a></li>
          <li><strong>Evening:</strong> Flight to Copenhagen</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">15</div>
          <h4>Jan 3: Departure <img src="https://cdn-icons-png.flaticon.com/512/825/825454.png" class="transport-icon" alt="Flight"></h4>
        </div>
        <ul>
          <li>Flight home from Copenhagen</li>
        </ul>
      </div>
    </section>

    <section id="logistics" class="section">
      <h2>📌 Travel Logistics</h2>
      <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div>
          <h3>Essential Bookings</h3>
          <ul>
            <li><a href="https://www.tivoli.dk/en/" target="_blank">Tivoli Gardens Tickets</a></li>
            <li><a href="https://www.legoland.dk/en/" target="_blank">LEGOLAND Billund</a></li>
            <li><a href="https://www.bluelagoon.com/" target="_blank">Blue Lagoon</a> (Dec 25)</li>
            <li><a href="https://santaclausvillage.info/" target="_blank">Santa Claus Village</a></li>
          </ul>
        </div>
        <div>
          <h3>Transportation</h3>
          <ul>
            <li><a href="https://www.dsb.dk/en/" target="_blank">Danish Trains (DSB)</a></li>
            <li><a href="https://www.vr.fi/en" target="_blank">Finnish Trains (VR)</a></li>
            <li><a href="https://www.tallinksilja.com/" target="_blank">Tallink Silja Ferries</a></li>
          </ul>
        </div>
        <div>
          <h3>Weather Prep</h3>
          <ul>
            <li>Denmark: 0°C to 5°C (rain/snow)</li>
            <li>Iceland: -5°C to 2°C (windy)</li>
            <li>Finland: -15°C to -5°C (snow)</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="gallery" class="section">
      <h2>📸 Photo Gallery</h2>
      <div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(250px, 1fr)); gap: 20px; margin-top: 1.5rem;">
        <div style="position: relative; overflow: hidden; border-radius: 8px; height: 200px; box-shadow: var(--shadow);">
          <img src="https://images.unsplash.com/photo-1513622470522-26c3c8a854bc?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Nyhavn, Copenhagen" style="width: 100%; height: 100%; object-fit: cover;">
          <div style="position: absolute; bottom: 0; left: 0; right: 0; background: rgba(0,0,0,0.7); color: white; padding: 10px;">
            <a href="https://www.visitcopenhagen.com/copenhagen/nyhavn-gdk410881" target="_blank" style="color: white;">Nyhavn, Copenhagen</a>
          </div>
        </div>
        <div style="position: relative; overflow: hidden; border-radius: 8px; height: 200px; box-shadow: var(--shadow);">
          <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Tivoli Gardens" style="width: 100%; height: 100%; object-fit: cover;">
          <div style="position: absolute; bottom: 0; left: 0; right: 0; background: rgba(0,0,0,0.7); color: white; padding: 10px;">
            <a href="https://www.tivoli.dk/en/" target="_blank" style="color: white;">Tivoli Gardens</a>
          </div>
        </div>
        <div style="position: relative; overflow: hidden; border-radius: 8px; height: 200px; box-shadow: var(--shadow);">
          <img src="https://images.unsplash.com/photo-1507272931001-fc06c17e4f43?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Northern Lights" style="width: 100%; height: 100%; object-fit: cover;">
          <div style="position: absolute; bottom: 0; left: 0; right: 0; background: rgba(0,0,0,0.7); color: white; padding: 10px;">
            <a href="https://en.visiticeland.com/plan-your-trip/northern-lights/" target="_blank" style="color: white;">Northern Lights</a>
          </div>
        </div>
        <div style="position: relative; overflow: hidden; border-radius: 8px; height: 200px; box-shadow: var(--shadow);">
          <img src="https://images.unsplash.com/photo-1579033462043-0f11a7862f7d?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Santa Village" style="width: 100%; height: 100%; object-fit: cover;">
          <div style="position: absolute; bottom: 0; left: 0; right: 0; background: rgba(0,0,0,0.7); color: white; padding: 10px;">
            <a href="https://santaclausvillage.info/" target="_blank" style="color: white;">Santa Claus Village</a>
          </div>
        </div>
      </div>
    </section>
  </div>

  <footer>
    <div class="container">
      <p>Northern Europe Family Adventure | December 2024</p>
      <p>Created with ❤️ for our amazing family</p>
    </div>
  </footer>

  <script>
    // Smooth scrolling for navigation
    document.querySelectorAll('nav a').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        
        document.querySelectorAll('nav a').forEach(a => {
          a.classList.remove('active');
        });
        this.classList.add('active');
        
        const targetId = this.getAttribute('href');
        document.querySelector(targetId).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });
    
    // Highlight current section in nav
    window.addEventListener('scroll', function() {
      const sections = document.querySelectorAll('section');
      let current = '';
      
      sections.forEach(section => {
        const sectionTop = section.offsetTop;
        const sectionHeight = section.clientHeight;
        
        if (pageYOffset >= sectionTop - 100) {
          current = section.getAttribute('id');
        }
      });
      
      document.querySelectorAll('nav a').forEach(a => {
        a.classList.remove('active');
        if (a.getAttribute('href') === `#${current}`) {
          a.classList.add('active');
        }
      });
    });
  </script>
</body>
</html>
