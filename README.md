# Ex.07 Restaurant Website
## Date:22/10/2025

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
```
rest.html


<html>
    <head>
        <title>
            DRIZZLE RESTAURANT
        </title>
        <link rel="stylesheet" href="rest.css">
    </head>
    <body>
        <div class="title">
            <p>DRIZZLE RESTAURANT</p>
        </div>
        <div class="quote">
            <p>Satisfy your cravings in style.</p>
        </div>
        <div class="link">
            <a href="rest.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="admin.html">Administration</a>
            <a href="contact.html">Contact</a>
        </div>
        <div class="footer">&copy; INDHUJA.K - 25018219</div>
    </body>
</html>


rest.css


body{
    background-image: url('home.png');
    background-repeat: no-repeat;
    background-size: cover;
    justify-content: space-between;
    display: flex;
}
.title{
    position: fixed;
    top:0;
    font-family:'Courier New', Courier, monospace;
    margin-left: 5px;
    font-size:80px;
    font-weight: bolder;
    color:rgb(255, 252, 252)
}
.quote{
    position: absolute;
    bottom: 60%;
    margin-left: 5px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: bolder;
    font-size: 30px;
    color:rgb(255, 254, 254)
}


.link{
    position: fixed;
    top:0;
    @media(any-hover: hover){
        a:hover{
            background-color: rgb(255, 222, 4);
        }
    }
    margin-top: 40px;
    margin-left: 1040px;
    margin-right: 50px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 22px;
}
.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  background-color: rgb(246, 201, 0);
  color: rgb(0, 0, 0);
  text-align: center;
  padding: 10px;
}

menu.html

<html>
    <head>
        <title>
            Menu: DRIZZLE
        </title>
        <link rel="stylesheet" href="menu.css">
        <body>
            <div class="link">
                <a href="rest.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="admin.html">Administration</a>
                <a href="contact.html">Contact</a>
            </div>
            <div class="title">
                <p>DRIZZLE Menu</p>
            </div>
            <div class="menu-grid">
                <div class="menu-item">
                    <img src="biriyani.jpg">
                    <h3>Biriyani - 100$</h3>
                </div>
                <div class="menu-item">
                    <img src="shawarma.jpg">
                    <h3>Shawarma - 50$</h3>
                </div>
                <div class="menu-item">
                    <img src="cholabhatura.jpg">
                    <h3>Chola Bhatura - 70$</h3>
                </div>
                <div class="menu-item">
                    <img src="parotta.jpg">
                    <h3>Parotta  - 80$</h3>
                </div>
                <div class="menu-item">
                    <img src="momos.jpg">
                    <h3>Momos - 50$</h3>
                </div>
                <div class="menu-item">
                    <img src="dumpling.jpg">
                    <h3>Dumpling - 50$</h3>
                </div>
                <div class="menu-item">
                    <img src="lollipop.jpg">
                    <h3>Chicken Lolipop - 80$</h3>
                </div>
                <div class="menu-item">
                    <img src="ramen.jpg">
                    <h3>Ramen - 100$</h3>
                </div>
                <div class="menu-item">
                    <img src="sushi.jpg">
                    <h3>Sushi - 90$</h3>
                </div>
                <div class="menu-item">
                    <img src="butterchicken.jpg">
                    <h3>Butter chicken - 80$</h3>
                </div>
                <div class="menu-item">
                    <img src="noodle.jpg">
                    <h3>Noodle - 90$</h3>
                </div>
                <div class="menu-item">
                    <img src="friedrice.jpg">
                    <h3>Fried Rice - 90$</h3>
                </div>
            </div>
            <div class="footer">&copy; INDHUJA.K - 25018219</div>
        </body>
    </head>
</html>


menu.css

body{
    background-image: url('bg.png');
    background-repeat: no-repeat;
    background-size: cover;
    justify-content: space-between;
    display: flex;
}
.title{
    position: relative;
    top:0;
    font-family:'Times New Roman', Times, serif;
    margin-left: 5px;
    font-size:60px;
    font-weight: bolder;
    color:rgb(255, 255, 255)
}
.link{
    position: fixed;
    top:0;
    @media(any-hover: hover){
        a:hover{
            background-color: rgb(255, 222, 4);
        }
    }
    margin-top: 40px;
    margin-left: 1040px;
    margin-right: 50px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 22px;
}
.menu-grid{
    align-items: center;
    display: grid;
    grid-template-columns: repeat(6,1fr);
    gap: 10px;
    padding: 20px;
    background-size: 80%;
    background-color: rgba(131, 111, 115, 0.6);
}
.menu-item {
  background-color: rgb(255, 234, 0);
  background-size: 700px;
  padding: 1px;
  border-radius: 5px;
  text-align: center;
  border: 2px solid #000000;
}
.menu-item img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  margin-bottom: 5px;
}
.menu-item h3 {
  margin: 0;
  font-size: 20px;
  color: #000000;
}
.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  background-color: rgb(254, 195, 0);
  color: rgb(0, 0, 0);
  text-align: center;
  padding: 10px;
}

admin.html

<html>
    <head>
        <title>
            Administration: DRIZZLE
        </title>
        <link rel="stylesheet" href="admin.css">
    </head>
    <body>
        <div class="link">
            <a href="rest.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="admin.html">Administration</a>
            <a href="contact.html">Contact</a>
        </div>
        <div class="title">
            <p>DRIZZLE - TEAM</p>
        </div>
        <div class="team-grid">
            <div class="team-item">
                <img src="indhuja.jpg">
                <h2>INDHUJA.K</h2>
                <p>CEO</p>
            </div>
            <div class="team-item">
                <img src="lisa.jpg">
                <h2>LISA</h2>
                <p>Manager</p>
            </div>
            <div class="team-item">
                <img src="jennie.jpg">
                <h2>JENNIE</h2>
                <p>Head Cheif</p>
            </div>
            <div class="team-item">
                <img src="selena.jpg">
                <h2>SELENA GOMEZ</h2>
                <p>Food Scientist</p>
            </div>
            <div class="team-item">
                <img src="ariana.jpg">
                <h2>ARIANA GRANGY</h2>
                <p>HR Manager</p>
            </div>
            <div class="team-item">
                <img src="zendaya.jpg">
                <h2>ZENDAYA</h2>
                <p>security Head</p>
            </div>
        </div>
        <div class="footer">&copy; INDHUJA.K - 25018219</div>
    </body>
</html>


admin.css

body{
    background-image: url('admin.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    justify-content: space-between;
    display: flex;
}
.title{
    position: absolute;
    top:0;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    margin-left: 5px;
    font-size:60px;
    font-weight: bolder;
    color:rgb(255, 255, 255)
}
.link{
    position: fixed;
    top:0;
    @media(any-hover: hover){
        a:hover{
            background-color: rgb(255, 225, 0);
        }
    }
    margin-top: 40px;
    margin-left: 1040px;
    margin-right: 50px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 22px;
}
.team-grid{
    align-items: center; 
    bottom:0;
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 30px;
    padding: 40px;
    max-width: 1200px;
    margin: 0 auto;
}

.team-item {
  background-color: rgb(251, 255, 0);
  background-size: 200px;
  border-radius: 5px;
  text-align: center;
  border: 2px solid #000000;
  margin-top: 200px;
  height: 250px;
}
.team-item img {
  width: 120px;
  height: auto;
  border-radius: 50%;
  border: 3px solid rgb(92, 90, 91);
  margin-bottom: 20px;
  margin-left: auto;
  margin-right: auto;
}
.team-item h2{
  margin: 0;
  font-size: 20px;
  color: rgb(0, 0, 0);
}
.team-item p{
    margin: 0;
    font-size: 20px;
    color:rgb(39, 35, 35)
}
.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  background-color: rgb(255, 230, 0);
  color: rgb(0, 0, 0);
  text-align: center;
  padding: 10px;
}


contact.html

<html>
    <head>
        <title>
            Contact-us: DRIZZLE
        </title>
        <link rel="stylesheet" href="contact.css">
    </head>
    <body>
        <div class="link">
                <a href="rest.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="admin.html">Administration</a>
                <a href="contact.html">Contact</a>
        </div>
        <div class="title">
            <p>DRIZZLE RESTAURANT</p>
        </div>
        <div class="box">
            <h2>Contact details</h2>
            <p>Meet Us at:</p>
            <p>279-XXX street chennai</p>
            <p>Phone: +91 27638 66778</p>
            <p>Email: drizzle@gmail.com</p>
        </div>
        <div class="footer">&copy; INDHUJA.K - 25018219</div>
    </body>
</html>

contact.css

body{
    background-image: url('bg.png');
    background-repeat: no-repeat;
    background-size: cover;
    justify-content: space-between;
    display: flex;
    align-items: center;
}
.title{
    position: absolute;
    top:0;
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    margin-left: 5px;
    font-size:60px;
    font-weight: bolder;
    color:rgb(245, 245, 245)
}
.link{
    position: fixed;
    top:0;
    @media(any-hover: hover){
        a:hover{
            background-color: rgb(255, 222, 4);
        }
    }
    margin-top: 40px;
    margin-left: 1040px;
    margin-right: 50px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 22px;
}
.box{
    margin-left:600px; 
    border: solid rgb(255, 234, 0); 
    background-color: rgb(69, 69, 69);
    width:250px; 
    height:auto; 
    text-align:center; 
    padding:20px;
}
.box h2{
    font-size: 35px;
    color:rgb(255, 255, 255);
}
.box p{
    font-size: larger;
    color:rgb(221, 221, 221);
}
.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  background-color: rgb(251, 255, 0);
  color: rgb(0, 0, 0);
  text-align: center;
  padding: 10px;
}


```

## OUTPUT:

![alt text](<Screenshot (45).png>)
![alt text](<Screenshot (46).png>)
![alt text](<Screenshot (47).png>)
![alt text](<Screenshot (49).png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
