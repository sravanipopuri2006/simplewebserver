# EX01 Developing a Simple Webserver
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
## HTML CODE
```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <header>
        <div class="navbar">
            <div class="nav-logo border" >
                <div class="logo"></div>
            </div>
            <div class="nav-address border">
                <p class="first">Deliver to</p>
                <div class="add-icon">
                    <i class="fa-solid fa-location-dot"></i>
                    <p class="second">India</p>
                </div>
            </div>
            <div class="searchbox">
                <select class="search-select">
                    <option value="All">All</option>

                </select>
                <input type="text" placeholder="Search Amazon" class="input-text">
                <div class="search-logo">
                    <i class="fa-solid fa-magnifying-glass"></i>
                </div>
            </div>
            <div class="nav-signin border">
                <p><span>Hello,sign in</span></p>
                <p class="nav-second">Account & Lists</p>

            </div>
            <div class="nav-orders border">
                <p><span>Returns</span></p>
                <p class="nav-second">& Orders</p>

            </div>
            
            <div class="cart-logo border">
                <i class="fa-solid fa-cart-shopping"></i>
                <p>Cart</p>
             </div>
                
            
        </div>
        <div class="nav-panel">
            <div class="nav-menu border">
                <i class="fa-solid fa-bars"></i>
                <p>All</p>
            </div>
            <div class="list-menu ">
                <p class="border">Today'S Deals</p>
                <p class="border">Customer Service</p>
                <p class="border">Registry</p>
                <p class="border">Gift Cards</p>
                <p class="border">Sell</p>
                
            </div>
            <div class="shop border">
                <p>Shop deals in Electronics</p>
            </div>

        </div>
    </header>
    <div class="hero-section">
        <div class="hero-msg"><p>You are on amazon.com. You can also shop on Amazon India for millions of products with fast local delivery. <a>Click here to go to amazon.in</a></p></div>
    </div>
    <div class="shop-section">
        <div class="box1 box">
            <div class="box-content">
                <h2>Health & Personal Care</h2>
                <div class="box-img" style="background-image: url('box1_image.jpg'); "></div>
                <p>See More</p>
            </div>
            
        </div>
        <div class="box2 box">
            <div class="box-content">
                <h2>Personal Care</h2>
                <div class="box-img" style="background-image: url('box2_image\ .jpg'); "></div>
                <p>See More</p>
            </div>
        </div>
        <div class="box3 box">
            <div class="box-content">
                <h2>Furniture</h2>
                <div class="box-img" style="background-image: url('box3_image.jpg'); "></div>
                <p>See More</p>
            </div>
        </div>
        <div class="box4 box">

            <div class="box-content">
                <h2>Electronics</h2>
                <div class="box-img" style="background-image: url('box4_image.jpg'); "></div>
                <p>See More</p>
            </div>
        </div>
        <div class="box5 box">
            <div class="box-content">
                <h2>Make up & Beauty</h2>
                <div class="box-img" style="background-image: url('box5_image.jpg'); "></div>
                <p>See More</p>
            </div>

        </div>
        <div class="box6 box">
            <div class="box-content">
                <h2>Pets</h2>
                <div class="box-img" style="background-image: url('box6_image.jpg'); "></div>
                <p>See More</p>
            </div>

        </div>
        <div class="box7 box">
            <div class="box-content">
                <h2>Toys</h2>
                <div class="box-img" style="background-image: url('box7_image.jpg'); "></div>
                <p>See More</p>
            </div>

        </div>
        <div class="box8 box">
            <div class="box-content">
                <h2>Clothes & Fashion</h2>
                <div class="box-img" style="background-image: url('box8_image.jpg'); "></div>
                <p>See More</p>
            </div>

        </div>
    </div>
    
</body>
<footer>
    <div class="nav-footer">
        <p>Back to Top</p>
    </div>
    <div class="footpanel-2">
        <ul>
        <p>Get to Know Us</p>
        <a href="">Careers</a>  
        <a href="">Blog</a> 
        <a href="">About Amazon</a>  
        <a href="">Investor Relations</a>
        <a href=""> Amazon Devices</a>
        <a href="">Amazon Science</a> 
    </ul>
    <ul>
        <p>Get to Know Us</p>
        <a href="">Careers</a>  
        <a href="">Blog</a> 
        <a href="">About Amazon</a>  
        <a href="">Investor Relations</a>
        <a href=""> Amazon Devices</a>
        <a href="">Amazon Science</a> 

    </ul>
    <ul>
        <p>Get to Know Us</p>
        <a href="">Careers</a>  
        <a href="">Blog</a> 
        <a href="">About Amazon</a>  
        <a href="">Investor Relations</a>
        <a href=""> Amazon Devices</a>
        <a href="">Amazon Science</a> 
    </ul>
    <ul>
        <p>Get to Know Us</p>
        <a href="">Careers</a>  
        <a href="">Blog</a> 
        <a href="">About Amazon</a>  
        <a href="">Investor Relations</a>
        <a href=""> Amazon Devices</a>
        <a href="">Amazon Science</a> 
    </ul>

    </div>
    <div class="footpanel-3">
        <div class="foot-logo border"></div>
    </div>
    <div class="footpanel-4">
        <div class="foot-content">
            <p>Conditions of use</p>
            <p>Privacy Notice</p>
            <p>Your Ads Privacy Choice</p>
            

        </div>
        <div class="foot-copy">
            <p>© 1996-2024, Amazon.com, Inc. or its affiliates</p>
        </div>
    </div>
</footer>
</html>

## CSS CODE


*{
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
    
    
}
.navbar{
    height: 60px;
    background-color: #0F1111;
    color: white;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
}
.nav-logo{
    height: 50px;
    width: 100px;

}
.logo{
    
    background-image: url("amazon_logo.png");
    background-size: cover;
    height: 50px;
    width: 100%;

}
.border{
    border: 1.5px solid transparent;
}

.border:hover{
    border: 1.5px solid white;
}
.first{
    font-size: 0.85rem;
    color: #cccccc;
    margin-left: 15px;
}
.second{
    font-size: 1rem;
    margin: 3px;
    
}
.add-icon{
    display:flex;
    align-items: center;
   
}

.searchbox{
   width: 620px;
    display: flex;
    background-color: pink;
    height: 40px;
    border-radius: 4px;
    justify-content: space-evenly;
    

}
.search-select{
    border-top-left-radius: 4px;
    border-bottom-right-radius: 4px;
    background-color: #E6E6E6;
    width: 50px;
    text-align: center;
    border: none;
}
.input-text{
    width: 100%;
    font-size: 1rem;

}
.search-logo{
    width: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    background-color: rgb(255, 162, 0);
    border-top-right-radius: 4px;
    border-bottom-right-radius: 4px;
    color: #0F1111;
}
span{
    font-size: 12px;

}
.nav-second{
    font-size: 14px;
    font-weight: 700;
}
.cart-logo{
    display: flex;
    align-items: center;
    font-weight: 700;
    
}
.cart-logo i{
    font-size: 35px;
    
}
.searchbox:active{
    border: 3.6px orange solid;
}
.nav-panel{
    background-color: #222f3d;
    height: 40px;
    display: flex;
    color: #ffffff;
    align-items: center;
    justify-content: space-evenly;
    
}
.nav-menu{
    display: flex;
   
    

    
}
.list-menu{
    
    display: flex;
    font-size: 0.85rem;
    width: 70%;
}
.list-menu p{
    margin-left: 15px;
}
.shop{
    font-size: 0.9rem;
    font-weight: 700;
}
.hero-section{
    background-image: url("hero_image.jpg");
    height: 350px;
    background-size: cover;
    justify-content: center;
    display: flex;
    align-items: flex-end;


}
.hero-msg{
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: white;
    font-size: 0.85rem;
    width: 80%;
    margin-bottom: 25px;
    
}
.hero-msg a{
    color: #007185;
    
}
.shop-section{
    display: flex;
    justify-content: space-evenly;
    background-color: #e2e6e7;
    flex-wrap: wrap;
}
.box{
    height: 400px;
    width: 23%;
    background-color: white;
    
    padding: 20px 0px 15px;
    margin-top: 15px;
}
.box-img{
    height: 300px;
    background-size: cover;
    background-repeat: no-repeat;
    margin-top: 1rem;
    margin-bottom: 1rem;

}
.box-content{
    margin-left: 1rem;
    margin-right: 1rem;
}
.box-content p{
    color: #007185;
}
.nav-footer{
    height: 50px;
    background-color:#222f3d ;
    align-items: center;
    justify-content: center;
    display: flex;
    color: white;
}
.footpanel-2{
    display: flex;
    justify-content: space-evenly;
    background-color: #232F2E;
    height: 300px;
    

}
.footpanel-2 p{
    margin-top: 15px;
    color: white;
    margin-top: 20px;
}
.footpanel-2 a{
    text-decoration: none;
    color: white;
    display: block;
    font-size: 0.85rem;
    margin-top: 10px;
    color: #dddddd;
}
.footpanel-3{
    height: 70px;
    
   
    background-color:  #232F2E;
    border-top: 0.2px solid white;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;

}
.foot-logo{
    
    background-image: url(amazon_logo.png);
    width: 100px;
    height: 70px;
   
    background-size: contain;

}
.footpanel-4{
    background-color: #131a22;
    height: 80px;
    display: block;
    align-items: center;
    justify-content: center;
    color: white;

}

.foot-content{
   display: flex;
   align-items: center;
    justify-content: center;
    padding-top: 15px;
    font-size: 0.7rem;
}
.foot-copy{
    display: flex;
    align-items: center;
    justify-content: center;
    padding-top: 5px;
    font-size: 0.7rem;

    
    
}




## OUTPUT:


## RESULT:
The program for implementing simple webserver is executed successfully.
