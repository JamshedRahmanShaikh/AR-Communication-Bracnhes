# AR-Communication-Bracnhes
"Scan here to find our nearest AR Communication branch, contact details, and shop timings."
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AR Communication</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      min-height: 100vh;
      background-color: #c41e3a;
      background-image: url('Images/Back Ground.png');
      background-size: cover;
      background-position: center;
      background-repeat: repeat;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      font-family: Arial, Helvetica, sans-serif;
      padding: 20px;
      position: relative;
      overflow-x: hidden;
    }
    
    body::before {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(196, 30, 58, 0.15);
      pointer-events: none;
      z-index: 0;
    }
    
    .header {
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 30px;
      margin-bottom: 60px;
      z-index: 1;
      text-align: center;
    }
    
    .logo {
      width: 500px;
      max-width: 90vw;
      height: auto;
      filter: drop-shadow(0 0 8px rgba(0,0,0,0.4));
    }
    
    .logo img {
      width: 100%;
      height: auto;
      display: block;
    }
    
    .buttons {
      display: flex;
      flex-direction: column;
      gap: 35px;
      z-index: 1;
      width: 100%;
      max-width: 480px;
      padding: 0 15px;
    }
    
    .branch-btn {
      display: flex;              /* CHANGE 1: Changed from 'block' to 'flex' */
      align-items: center;        /* CHANGE 2: Added to center icon and text */
      justify-content: center;    /* CHANGE 3: Added to center content */
      width: 100%;
      padding: 22px 30px;
      background: #000;
      color: #fff;
      font-size: clamp(1.4rem, 5vw, 1.9rem);
      font-weight: 700;
      text-align: center;
      text-decoration: none;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      box-shadow: 0 6px 20px rgba(0,0,0,0.45);
      transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
      letter-spacing: 0.5px;
      gap: 10px;                  /* CHANGE 4: Added space between icon and text */
    }
    
    /* CHANGE 5: Added this new CSS class for the location icon */
    .location-icon {
      width: 25px;
      height: 25px;
      fill: #ffffff;
      flex-shrink: 0;
    }
    
    .branch-btn:hover {
      background: #1a1a1a;
      transform: translateY(-3px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.55);
    }
    
    .branch-btn:active {
      transform: translateY(1px);
      box-shadow: 0 4px 12px rgba(0,0,0,0.4);
    }
    
    @media (max-width: 600px) {
      .logo {
        width: 350px;
      }
      .buttons {
        gap: 25px;
      }
      .location-icon {
              width: 30px;    /* INCREASED FROM 20px */
              height: 30px;   /* INCREASED FROM 20px */
      }
    }
  </style>
</head>
<body>
  <div class="header">
    <div class="logo">
      <img src="Images/logo.png" alt="AR Communication Logo">
    </div>
  </div>
  
  <div class="buttons">
    <!-- CHANGE 6: Added location icon SVG inside First Branch button -->
    <a href="https://www.google.com/maps/place/AR+Communication/@24.9208242,67.1467276,17z/data=!3m1!4b1!4m6!3m5!1s0x3eb339000dc6b679:0xd0b683b58e62ea27!8m2!3d24.9208243!4d67.1515985!16s%2Fg%2F11vpzfwdr7?authuser=0&entry=ttu&g_ep=EgoyMDI2MDkyMC4wIKXMDSoASAFQAw%3D%3D"
       class="branch-btn"
       target="_blank"
       rel="noopener noreferrer">
       
      <svg class="location-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" hight="100pxl">
        <path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/>
      </svg>
      
      First Branch
    </a>
    
    <!-- CHANGE 7: Added location icon SVG inside 2nd Branch button -->
    <a href="https://www.google.com/maps/place/AR+communication+2nd+Branch/@24.9195332,67.1300959,17z/data=!3m1!4b1!4m6!3m5!1s0x3eb3390078028bbf:0x2cd96eb22cb628c4!8m2!3d24.9195332!4d67.1326708!16s%2Fg%2F11z9vpllf9?entry=ttu&g_ep=EgoyMDI2MDkyMC4wIKXMDSoASAFQAw%3D%3D"
       class="branch-btn"
       target="_blank"
       rel="noopener noreferrer">
       
      <svg class="location-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/>
      </svg>
      
      2nd Branch
    </a>
  </div>
</body>
</html>
