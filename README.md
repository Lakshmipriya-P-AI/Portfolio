# EXP 01 - PORTFOLIO

## AIM:

To create a portfolio using HTML and CSS

## ALGORITHM:

1. Set up the basic structure of your HTML document.

2. Create a CSS file named "styles.css" and link it to your HTML document. This file will contain the CSS rules for styling your portfolio.

3. Design the layout of your portfolio using HTML elements such as < header >, < nav >, < section >, < article >, and < footer >. Use appropriate classes or IDs to style these elements later with CSS.

4. Add a header section to display your name or the title of your portfolio.

5. Add images or media to enhance your portfolio. You can use the <img> tag to display images and embed videos or other media using appropriate HTML tags.

6. Apply responsive design techniques to ensure your portfolio looks good on different devices and screen sizes. Use CSS media queries to adjust the layout and styling as needed.

7. Apply CSS styling to your portfolio elements by targeting their respective classes or IDs in the "styles.css" file. Customize the colors, fonts, spacing, and other visual properties to match your desired design.

## CODE:

### HTML CODE:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PortFolio Website</title>
    <link rel="stylesheet" type="text/css" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <!---hero section start--->
    <div class="hero">
        <nav>
            <h2 class="logo">Port<span>Folio</span></h2>
            <ul>
                <li><a href="#about">Home</a></li>
                <li><a href="#service">About Us</a></li>
                <li><a href="#Skills">Skills</a></li>
                <li><a href="#contactme">Services</a></li>
            </ul>
        </nav>

        <div class="content">
            <h4>Hello, My name is</h4>
            <h1>Lakshmi <span>Priya</span></h1>
            <h3>I am an AI Student</h3>
            <div class="newsletter">
                <form>
                    <input type="email" name="email" id="mail" placeholder="Enter your Email">
                    <input type="submit" name="submit" value="Lets Start">
                </form>
            </div>
        </div>
    </div>

    <!-- About section start -->
    <section class="about">
        <div class="main">
            <img src="about.png">
            <div class="about-text">
                <h2>About Me</h2>
                <h5>In<span> AI </span> Profession </h5>
                <p>I am an AI Student with great passion
                    for all things supporting artificial
                    intelligence jobs. I consider myself a
                    responsible and hardworking person.
                    am looking forward for my first work
                    experience.Innovative Artificial Intelligence with application design,developement,testing and deployment.Highly experienced in writinh codes and algorithms s well asbuilding complex neural networks through various programming languages.Possess an unbridled passion for AI with comprehensive knowledge of Machine Learning concepts and advanced technology solutions through C#,C++,Javascript,Python for continuous inprovement of AI technologies..!!!</p>
                <button type="button">Let's Talk</button>
            </div>
        </div>    
    </section>

    <!-- service section start -->
    <div class="service">
        <div class="title">
            <h2>Profile</h2>
        </div>
        <div class="box">
            <div class="card">
                <i class="fa-solid fa-bars"></i>
                <h5>Skills</h5>
                <div class="pra">
                    <li>Html & Css</li>
                    <li>Python</li>
                    <li>C Programming</li>
                    <li>Product Developement</li>
                    <li>3D Designing</li>
                    <li>Data Science</li>
                    <li>Image Processing</li>
                    <p style="text-align: center;">
                    </p>
                </div>
            </div>

            <div class="card">
                <i class="fa-solid fa-pen-nib"></i>
                <h5>SoftSkills</h5>
                <div class="pra">
                    <li>Self-motivated</li>
                    <li>Adaptable</li>
                    <li>Problem Solving</li>
                    <li>Team Work</li>
                    <li>Time Management</li>
                    <li>Communication</li>
                    <li>Creative thinking</li>
                    <p style="text-align: center;">
                    </p>
                </div>
            </div>

            <div class="card">
                <i class="fa-solid fa-briefcase"></i>
                <h5>Career Objective</h5>
                <div class="pra">
                    <p style="text-align: center;">
                    <p>To work in a challenging environment
                        that provides ground to implement my
                        expertise and creativity.Seeking a challenging position in a reputed organization where I can learn new skills, expand my knowledge, and leverage my learnings.</p>
                    </p>
                </div>
            </div>
        </div>
    </div>


    <!-- footer -->
    <footer>
        <p>Contact Me</p>
        <div class="social">
            
            <a href="https://github.com/Lakshmipriya-P-AI"><i class="fa-brands fa-github"></i></a>
            <a href="https://www.linkedin.com/in/lakshmi-priya-6a0898271"><i class="fa-brands fa-linkedin"></i></a>
            <a href="https://mail.google.com/mail/?view=cm&source=mailto&to=plakshmipriya82@gmail.com@gmail.com"><i class="fa-solid fa-envelope"></i></a>
        </div>
        <p class="end">Copyright @2023  priya</p>
    </footer>
</body>
</html>
```
### CSS CODE:
```
*{
    padding: 0;
    margin: 0;
    font-family: 'Josefin Sans', sans-serif;
    box-sizing: border-box;
}

.hero{
    height: 100vh;
    width: 100%;
    background-image: url("back.png");
    background-size: cover;
    background-position: center;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 45px;
    padding-left: 8%;
    padding-right: 8%;
}

.logo{
    color: white;
    font-size: 35px;
    letter-spacing: 1px;
    cursor: pointer;
}
span{
    color:#9f2024;
}

nav ul li{
    list-style-type: none;
    display: inline-block;
    padding: 10px 25px;
}

nav ul li a{
    color: white;
    text-decoration: none;
    font-weight: bold;
    text-transform: capitalize;
}

nav ul li a:hover{
    color: #f9004d;
    transition: .3s;
}

.btn{
    background-color: #f9004d;
    color: white;
    text-decoration: none;
    border: 2px solid transparent;
    font-weight: bold;
    padding: 10px 25px;
    border-radius: 30px;
    transition: transform .4s;
}

.btn:hover{
    transform: scale(1.2);
}

.content{
    position: absolute;
    top: 50%;
    left: 8%;
    transform: translateY(-50%);
}

h1{
    color: rgb(125, 57, 57);
    margin: 20px 0px 20px;
    font-size: 75px;
}

h3{
    color: rgb(96, 55, 55);
    font-size: 25px;
    margin-bottom: 50px;
}

h4{
    color: white;
    letter-spacing: 2px;
    font-size: 20px;
}

.newsletter{
    width: 380px;
    max-width: 100%;
    position: relative;
}

.newsletter form input:first-child{
    display: inline-block;
    width: 100%;
    padding: 14px 130px 14px 15px;
    border: 2px solid #f9004d;
    border-radius: 30px;
}

.newsletter form input:last-child{
    position: absolute;
    display: inline-block;
    outline: none;
    border: none;
    padding: 10px 30px;
    border-radius: 30px;
    background-color: #f9004d;
    color: white;
    box-shadow: 0px 0px 5px #000, 0px 0px 15px #858585;
    top: 6px;
    right: 6px;
}

.about{
    width: 100%;
    padding: 100px 0px;
    background-color: #6a4a3a;
}

.about img{
    height:auto;
    width: 430px;
    border-radius: 40px;
}

.about-text{
    width: 550px;

}

.main{
    width: 1130px;
    max-width: 95%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-around
}

.about-text h2{
    color: white;
    font-size: 75px;
    text-transform: capitalize;
    margin-bottom: 20px;
}

.about-text h5{
    color: white;
    letter-spacing: 2px;
    font-size: 22px;
    margin-bottom: 25px;
    text-transform: capitalize;
}

.about-text p{
    color: #fffefe;
    letter-spacing: 1px;
    line-height: 28px;
    font-size: 18px;
    margin-bottom: 45px;
}

button{
    background-color: #a41744;
    color: white;
    text-decoration: none;
    border: 2px solid transparent;
    font-weight: bold;
    padding: 13px 30px;
    border-radius: 30px;
    transition: .3s;
}

button:hover{
    background-color: transparent;
    border: 2px solid;
    cursor: pointer;
}

.service{
    background: #8b6c5c;
    width: 100%;
    padding: 100px 0px;
}

.title h2{
    color: rgb(255, 255, 255);
    font-size: 75px;
    width: 1130px;
    margin: 30px auto;
    text-align: center;
}

.box{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 400px;

}
.card{
    height: 365px;
    width: 335px;
    padding: 40px 35px;
    background:#ffffff;
    border-radius: 20px;
    margin: 15px;
    position: relative;
    overflow: hidden;
    text-align: center;
}

.card i{
    font-size: 40px;
    display: block;
    text-align: center;
    margin: 3px 0px;
    color: #f9004d;
}

h5{
    color: rgb(168, 59, 59);
    font-size: 23px;
    margin-bottom: 15px;
}
.pra li{
    color: #962A51;
    font-size: 16px;
    line-height: 7px;
    margin-bottom: 25px;
}
.pra p{
    color: #962A51;
    font-size: 16px;
    line-height: 27px;
    margin-bottom: 25px;

}

.card .button{
    background-color: #f9004d;
    color: white;
    text-decoration: none;
    border: 2px solid transparent;
    font-weight: bold;
    padding: 9px 22px;
    border-radius: 30px;
    transition: .3s;
}

.card .button:hover{
    background-color: transparent;
    border: 2px solid #f9004d;
    cursor: pointer;
}



footer{
    position: relative;
    width: 100%;
    height: 250px;
    background:#101010;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

footer p:nth-child(1){
    font-size: 30px;
    color: white;
    margin-bottom: 20px;
    font-weight: bold;
}

.social{
    display: flex;
}

.social a{
    width: 45px;
    height: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
    background:#f9004d ;
    border-radius: 50%;
    margin: 22px 10px;
    color: white;
    text-decoration: none;
    font-size: 20px;
}

.social a:hover{
    transform: scale(1.3);
    transition: .3s;
}

.end{
    position: absolute;
    color: #f9004d;
    bottom: 35px;
    font-size: 14px;
}
```
## OUTPUT:
![image](https://github.com/Lakshmipriya-P-AI/Portfolio/assets/93427923/f8656ccc-bdbb-4e52-b1e4-38560cf355db)

![image](https://github.com/Lakshmipriya-P-AI/Portfolio/assets/93427923/a85ac8ac-ac1f-48c5-b8b4-bd498b13f4e8)

![image](https://github.com/Lakshmipriya-P-AI/Portfolio/assets/93427923/23fbcf1b-63fd-49d3-bcec-962adca4b5c8)

![image](https://github.com/Lakshmipriya-P-AI/Portfolio/assets/93427923/6e04eea4-bd5b-4137-9233-4eea3bbbef74)


## RESULT:
Thus, a Portfolio is created using HTML and CSS.
