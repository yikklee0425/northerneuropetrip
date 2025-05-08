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
    
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 1.5rem;
    }
    
    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      height: 200px;
      box-shadow: var(--shadow);
      transition: transform 0.3s ease;
    }
    
    .gallery-item:hover {
      transform: translateY(-5px);
    }
    
    .gallery-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s ease;
    }
    
    .gallery-item:hover img {
      transform: scale(1.05);
    }
    
    .gallery-caption {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      background: rgba(0,0,0,0.7);
      color: white;
      padding: 10px;
      transform: translateY(100%);
      transition: transform 0.3s ease;
    }
    
    .gallery-item:hover .gallery-caption {
      transform: translateY(0);
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
      .gallery {
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
      }
      
      nav ul {
        flex-direction: column;
        align-items: center;
      }
      
      nav li {
        margin: 5px 0;
      }
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
        <li><a href="#overview" class="active">Overview</a></li>
        <li><a href="#itinerary">Itinerary</a></li>
        <li><a href="#destinations">Destinations</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#logistics">Logistics</a></li>
      </ul>
    </div>
  </nav>

  <div class="container">
    <section id="overview" class="section">
      <h2>Trip Overview</h2>
      <p>Join our family of seven on an unforgettable winter journey through Northern Europe! This 14-day adventure takes us through the festive streets of Copenhagen, the breathtaking landscapes of Iceland, and the magical winter wonderland of Finnish Lapland.</p>
      
      <div class="action-item">
        <div class="action-title">Family Highlights</div>
        <ul>
          <li>Kids (15+): LEGOLAND, Northern Lights, husky sledding</li>
          <li>Adults: Christmas markets, geothermal spas, design districts</li>
          <li>All Ages: Santa Claus Village, Tivoli Gardens, Blue Lagoon</li>
        </ul>
      </div>
    </section>

    <section id="itinerary" class="section">
      <h2>Complete 15-Day Itinerary</h2>
      
      <!-- DENMARK -->
      <h3>🇩🇰 Denmark (Dec 20-23)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">1</div>
          <h4>Dec 20: Arrival in Copenhagen</h4>
        </div>
        <ul>
          <li><strong>Morning:</strong> Flight arrival at CPH</li>
          <li><strong>Afternoon:</strong> <a href="https://www.visitcopenhagen.com/copenhagen/nyhavn-gdk410881" target="_blank">Nyhavn harbor</a> walk</li>
          <li><strong>Evening:</strong> <a href="https://www.tivoli.dk/en/" target="_blank">Tivoli Gardens</a> Christmas market</li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">2</div>
          <h4>Dec 21: LEGOLAND Adventure</h4>
        </div>
        <ul>
          <li><strong>All day:</strong> <a href="https://www.legoland.dk/en/" target="_blank">LEGOLAND Billund</a></li>
          <li><strong>Evening:</strong> Return to Copenhagen</li>
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

      <!-- ICELAND -->
      <h3>🇮🇸 Iceland (Dec 23-28)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">4</div>
          <h4>Dec 23: Fly to Reykjavík</h4>
        </div>
        <ul>
          <li><strong>Morning:</strong> Flight to KEF</li>
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

      <!-- FINLAND -->
      <h3>🇫🇮 Finland (Dec 28 - Jan 3)</h3>
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">9</div>
          <h4>Dec 28: Fly to Rovaniemi</h4>
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
          <h4>Dec 30: Travel to Levi</h4>
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
          <h4>Jan 1: Tallinn Day Trip</h4>
        </div>
        <ul>
          <li><a href="https://www.tallink.com/" target="_blank">Ferry to Tallinn</a></li>
          <li><a href="https://www.oldehansa.ee/" target="_blank">Medieval dinner at Olde Hansa</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">14</div>
          <h4>Jan 2: Helsinki Exploration</h4>
        </div>
        <ul>
          <li><a href="https://www.suomenlinna.fi/en/" target="_blank">Suomenlinna Fortress</a></li>
          <li><a href="https://www.loylyhelsinki.fi/en/" target="_blank">Löyly sauna</a></li>
        </ul>
      </div>
      
      <div class="itinerary-day">
        <div class="day-title">
          <div class="day-number">15</div>
          <h4>Jan 3: Departure</h4>
        </div>
        <ul>
          <li>Flight home from HEL</li>
        </ul>
      </div>
    </section>

    <!-- PHOTO GALLERY WITH WORKING IMAGES -->
    <section id="gallery" class="section">
      <h2>Photo Gallery</h2>
      <div class="gallery">
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1513622470522-26c3c8a854bc?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Nyhavn, Copenhagen">
          <div class="gallery-caption"><a href="https://www.visitcopenhagen.com/copenhagen/nyhavn-gdk410881" target="_blank">Nyhavn</a></div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Tivoli Gardens">
          <div class="gallery-caption"><a href="https://www.tivoli.dk/en/" target="_blank">Tivoli Gardens</a></div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1604977048617-3ab9e7c1e0c3?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="LEGOLAND">
          <div class="gallery-caption"><a href="https://www.legoland.dk/en/" target="_blank">LEGOLAND</a></div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1507272931001-fc06c17e4f43?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Northern Lights">
          <div class="gallery-caption"><a href="https://en.visiticeland.com/plan-your-trip/northern-lights/" target="_blank">Aurora Borealis</a></div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1544551763-7709d4037515?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Blue Lagoon">
          <div class="gallery-caption"><a href="https://www.bluelagoon.com/" target="_blank">Blue Lagoon</a></div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1579033462043-0f11a7862f7d?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Santa Village">
          <div class="gallery-caption"><a href="https://santaclausvillage.info/" target="_blank">Santa Claus Village</a></div>
        </div>
      </div>
    </section>

      <!-- ACTION ITEMS -->
      <div class="action-item">
        <div class="action-title">Critical Bookings Needed</div>
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px;">
          <div>
            <strong>Denmark:</strong>
            <ul>
              <li>Tivoli tickets (Dec 20)</li>
              <li>LEGOLAND tickets (Dec 21)</li>
            </ul>
          </div>
          <div>
            <strong>Iceland:</strong>
            <ul>
              <li>Blue Lagoon (Dec 25)</li>
              <li>Christmas dinner (Dec 24)</li>
            </ul>
          </div>
          <div>
            <strong>Finland:</strong>
            <ul>
              <li>Glass igloo (Dec 28-29)</li>
              <li>Tallinn ferry (Jan 1)</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
      

    <section id="destinations" class="section">
      <h2>Destination Highlights</h2>
      <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div>
          <h3>🇩🇰 Denmark</h3>
          <ul>
            <li>Tivoli Gardens Christmas market</li>
            <li>LEGOLAND Billund</li>
            <li>Nyhavn waterfront</li>
          </ul>
        </div>
        <div>
          <h3>🇮🇸 Iceland</h3>
          <ul>
            <li>Golden Circle tour</li>
            <li>Blue Lagoon geothermal spa</li>
            <li>Northern Lights hunting</li>
          </ul>
        </div>
        <div>
          <h3>🇫🇮 Finland</h3>
          <ul>
            <li>Santa Claus Village (Rovaniemi)</li>
            <li>Levi ski resort</li>
            <li>Tallinn day trip (Estonia)</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="gallery" class="section">
      <h2>Photo Gallery</h2>
      <div class="gallery">
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1513622470522-26c3c8a854bc?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Copenhagen Nyhavn">
          <div class="gallery-caption">Nyhavn, Copenhagen</div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Tivoli Gardens">
          <div class="gallery-caption">Tivoli Gardens</div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1604977048617-3ab9e7c1e0c3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="LEGOLAND">
          <div class="gallery-caption">LEGOLAND Billund</div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1507272931001-fc06c17e4f43?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Iceland Aurora">
          <div class="gallery-caption">Northern Lights</div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1544551763-7709d4037515?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Blue Lagoon">
          <div class="gallery-caption">Blue Lagoon</div>
        </div>
        <div class="gallery-item">
          <img src="https://images.unsplash.com/photo-1579033462043-0f11a7862f7d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Santa Village">
          <div class="gallery-caption">Santa Claus Village</div>
        </div>
      </div>
    </section>

    <section id="logistics" class="section">
      <h2>Travel Logistics</h2>
      <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
        <div>
          <h3>Flights</h3>
          <ul>
            <li>Copenhagen (CPH) arrival: Dec 20</li>
            <li>CPH → KEF (Iceland): Dec 23</li>
            <li>KEF → HEL (Finland): Dec 28/29</li>
            <li>HEL departure: Jan 3</li>
          </ul>
        </div>
        <div>
          <h3>Key Links</h3>
          <ul>
            <li><a href="https://www.tivoli.dk/en/" target="_blank">Tivoli Gardens Tickets</a></li>
            <li><a href="https://www.legoland.dk/en/" target="_blank">LEGOLAND Billund</a></li>
            <li><a href="https://www.bluelagoon.com/" target="_blank">Blue Lagoon Booking</a></li>
            <li><a href="https://www.visitrovaniemi.fi/" target="_blank">Rovaniemi Activities</a></li>
          </ul>
        </div>
      </div>
      
      <div class="action-item" style="margin-top: 20px;">
        <div class="action-title">Packing Checklist</div>
        <ul>
          <li>Thermal base layers</li>
          <li>Waterproof winter boots</li>
          <li>Swimsuit (for geothermal spas)</li>
          <li>Power adapters (EU plugs)</li>
        </ul>
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
    // Simple smooth scrolling for navigation
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
