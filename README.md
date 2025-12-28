# Ex.07 Restaurant Website
## Date:25.12.2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
home.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Taste Heaven Restaurant</title>
  <style>
    body{
      margin:0;
      padding:0;
      font-family:Arial, sans-serif;
      background-color:white;
    }

    header{
      background-image:url('rest.jpg');      /* Add your banner image */
      background-size:cover;
      background-position:center;
      text-align:center;
      padding:130px 20px;
      position:relative;
      color:white;
    }
    header::before{
      content:"";
      position:absolute;
      top:0;left:0;width:100%;height:100%;
      background:rgba(0,0,0,0.4);
      z-index:0;
    }
    header h1, header p{
      position:relative;z-index:1;
    }
    header h1{
      font-size:3.3em;
      letter-spacing:3px;
    }

    nav{
      text-align:center;
      background:black;
      padding:12px;
    }
    nav a{
      color:white;
      padding:12px 20px;
      text-decoration:none;
      font-size:17px;
      font-weight:bold;
    }
    nav a:hover{
      background:orange;
    }

    .section-container{
      display:flex;
      justify-content:center;
      gap:30px;
      flex-wrap:wrap;
      padding:50px;
    }

    .card{
      width:300px;
      background:white;
      border-radius:10px;
      box-shadow:0 4px 8px rgba(0,0,0,0.2);
      text-align:center;
      padding-bottom:15px;
      transition:0.3s;
    }
    .card:hover{
      transform:scale(1.05);
    }
    .card img{
      width:100%;
      height:200px;
      border-radius:10px 10px 0 0;
      object-fit:cover;
    }
    .card h2{
      margin:10px 0;
    }
    .card p{
      padding:0 12px;
      font-size:15px;
    }
    .card a{
      text-decoration:none;
      color:white;
      padding:8px 15px;
      background:orange;
      border-radius:5px;
      font-weight:bold;
    }
    .card a:hover{
      background:darkorange;
    }
  </style>
</head>

<body>

<header>
  <h1>TASTE HEAVEN</h1>
  <p>PURE DELICIOUS MOMENTS ON YOUR PLATE</p>
</header>

<nav>
  <a href="home.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="workers.html">Workers</a>
  <a href="contact.html">Contact</a>
</nav>

<section class="section-container">

  <div class="card">
    <img src="menu.jpg">
    <h2>Menu</h2>
    <p>Explore our delicious variety of meals.</p>
    <a href="menu.html">View</a>
  </div>

  <div class="card">
    <img src="worker.jpg">
    <h2>Our Workers</h2>
    <p>Meet our talented chefs and staff.</p>
    <a href="workers.html">View</a>
  </div>

  <div class="card">
    <img src="contact.png">
    <h2>Contact Us</h2>
    <p>Book your table or ask your queries.</p>
    <a href="contact.html">View</a>
  </div>

</section>

</body>
</html>

menu.html

<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Menu</title>
  <style>
    body{
      margin:0;
      padding:0;
      color:white;
      font-family:Arial;
    }
    header{
      background:black;
      padding:12px;
      text-align:center;
    }
    header a{
      color:white;padding:10px 15px;
      text-decoration:none;font-weight:bold;
    }
    header a:hover{background:orange;}

    .menu-container{
      display:flex;flex-wrap:wrap;
      justify-content:center;gap:20px;
      padding:40px;
      background:url('rest2.jpg');          /* Add image */
      background-size:cover;
    }
    .box{
      width:260px;
      background:rgba(0,0,0,0.7);
      padding:15px;border-radius:10px;
      backdrop-filter:blur(4px);
    }
    .box h2{color:orange;text-align:center;}
    .item{
      display:flex;justify-content:space-between;
      border-bottom:1px solid orange;
      padding:8px 0;
      font-size:17px;
    }
  </style>
</head>
<body>

<header>
  <a href="home.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="workers.html">Workers</a>
  <a href="contact.html">Contact</a>
</header>

<div class="menu-container">

  <div class="box">
    <h2>Breakfast</h2>
    <div class="item"><span>Idly</span><span>₹50</span></div>
    <div class="item"><span>Dosa</span><span>₹70</span></div>
    <div class="item"><span>Poori</span><span>₹60</span></div>
    <div class="item"><span>Upma</span><span>₹55</span></div>
  </div>

  <div class="box">
    <h2>Lunch</h2>
    <div class="item"><span>Meals</span><span>₹150</span></div>
    <div class="item"><span>Veg Biriyani</span><span>₹180</span></div>
    <div class="item"><span>Fried Rice</span><span>₹160</span></div>
    <div class="item"><span>Sambar Rice</span><span>₹120</span></div>
  </div>

  <div class="box">
    <h2>Desserts</h2>
    <div class="item"><span>Ice Cream</span><span>₹90</span></div>
    <div class="item"><span>Brownie</span><span>₹150</span></div>
    <div class="item"><span>Fruit Salad</span><span>₹120</span></div>
    <div class="item"><span>Gulab Jamun</span><span>₹80</span></div>
  </div>

</div>
</body>
</html>

workers.html

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Workers</title>
<style>
body{
  font-family:Arial;margin:0;padding:0;
  background:url('workersbg.jpg') center/cover no-repeat;
}
header{
  background:black;padding:12px;text-align:center;
}
header a{color:white;padding:10px 15px;text-decoration:none;font-weight:bold;}
header a:hover{background:orange;}

.container{
  display:flex;flex-wrap:wrap;gap:25px;
  justify-content:center;
  padding:40px;
}

.card{
  width:230px;background:white;padding:12px;border-radius:10px;
  text-align:center;box-shadow:0 4px 10px rgba(0,0,0,0.2);
}
.card img{
  width:100%;height:200px;border-radius:8px;object-fit:cover;
}
.card h3{margin:7px 0;}
.card p{font-size:14px;}
</style>
</head>
<body>

<header>
  <a href="home.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="workers.html">Workers</a>
  <a href="contact.html">Contact</a>
</header>

<div class="container">

  <div class="card">
    <h3>Master Chef Ragu</h3>
    <p>Specialist in South Indian Cuisine</p>
  </div>

  <div class="card">
    <h3>Chef Meera</h3>
    <p>Dessert Specialist</p>
  </div>

  <div class="card">
    <h3>John</h3>
    <p>Senior Waiter</p>
  </div>

</div>

</body>
</html>

contact.html

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Contact</title>
<style>
body{
  margin:0;padding:0;font-family:Arial;color:white;
  background:url('contactbg.jpg') center/cover no-repeat;
}
header{
  background:black;padding:12px;text-align:center;
}
header a{color:white;padding:10px 15px;text-decoration:none;font-weight:bold;}
header a:hover{background:orange;}

.form{
  width:350px;margin:80px auto;
  background:rgba(0,0,0,0.7);
  padding:25px;border-radius:10px;
}
.form h2{text-align:center;margin-bottom:15px;color:orange;}
.form input,textarea{
  width:100%;padding:10px;margin:7px 0;
  border:none;border-radius:5px;
}
button{
  width:100%;padding:10px;border:none;
  background:orange;font-size:18px;font-weight:bold;
}
button:hover{background:darkorange;}
</style>
</head>

<body>

<header>
  <a href="home.html">Home</a>
  <a href="menu.html">Menu</a>
  <a href="workers.html">Workers</a>
  <a href="contact.html">Contact</a>
</header>

<form class="form">
  <h2>Contact Us</h2>
  <input type="text" placeholder="Name" required>
  <input type="email" placeholder="Email" required>
  <input type="tel" placeholder="Phone" required>
  <textarea placeholder="Message..." rows="4"></textarea>
  <button>Submit</button>
</form>

</body>
</html>

## OUTPUT:
<img width="1044" height="522" alt="Screenshot 2025-12-28 155438" src="https://github.com/user-attachments/assets/2b4c353e-e35d-4e62-8acb-1bc225d5c3a8" />
<img width="1034" height="524" alt="Screenshot 2025-12-28 155508" src="https://github.com/user-attachments/assets/98bac141-6ce0-4a88-8204-898b5824bcce" />
<img width="1031" height="518" alt="Screenshot 2025-12-28 155525" src="https://github.com/user-attachments/assets/f3d46be8-6d9f-474c-950f-bd658c82b861" />
<img width="1044" height="560" alt="Screenshot 2025-12-28 155544" src="https://github.com/user-attachments/assets/8b91cbca-6dd7-4b3a-8a10-9bf7b8248641" />


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
