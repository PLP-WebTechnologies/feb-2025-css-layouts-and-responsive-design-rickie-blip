index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Webpage</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Navigation Bar -->
  <header class="navbar">
    <div class="logo">
      <h1>Week 4 plp web</h1>
    </div>
    <nav class="nav-links">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Main Content -->
  <main class="content">
    <section class="grid-container">
      <div class="grid-item">Name</div>
      <div class="grid-item">Address</div>
      <div class="grid-item">Email</div>
      <div class="grid-item">Contact</div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="footer">
    <p>&copy; 2025 PLP COHORT. All rights reserved.</p>
  </footer>

</body>
</html>
style.css
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  /* Body and General Layout */
  body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #23bb5d;
  }
  
  /* Navigation Bar */
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #0a2d44;
    color: white;
    padding: 20px;
  }
  
  .navbar .logo h1 {
    margin: 0;
  }
  
  .nav-links ul {
    list-style: none;
    display: flex;
    margin: 0;
  }
  
  .nav-links ul li {
    margin: 0 15px;
  }
  
  .nav-links ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
  }
  
  .nav-links ul li a:hover {
    text-decoration: underline;
  }
  
  /* Main Content Section */
  .content {
    padding: 20px;
  }
  
  /* Grid Layout */
  .grid-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
  }
  
  .grid-item {
    background-color: #fff;
    padding: 20px;
    border: 1px solid #ddd;
    text-align: center;
  }
  
  /* Footer */
  .footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
  }
  
  /* Media Query for Tablets (max-width 768px) */
  @media (max-width: 768px) {
    .grid-container {
      grid-template-columns: repeat(2, 1fr);
    }
  
    .nav-links ul {
      flex-direction: column;
      text-align: center;
    }
  
    .nav-links ul li {
      margin: 10px 0;
    }
  }
  
  /* Media Query for Mobile (max-width 480px) */
  @media (max-width: 480px) {
    .grid-container {
      grid-template-columns: 1fr;
    }
  
    .navbar {
      flex-direction: column;
      align-items: center;
    }
  
    .nav-links ul {
      flex-direction: column;
      text-align: center;
    }
  
    .nav-links ul li {
      margin: 10px 0;
    }
  }
  
