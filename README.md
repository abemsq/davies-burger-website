# Static Website: Typography

Aoife Conleavy is a novelist who has been writing about her travels for nearly two decades. Before the launch of her new novel Tide Blade, which features the stories of real-life characters in Morocco, the author wants to spruce up her professional website. You’ll modify the typography on her site, changing the size, style, and font families, to make the page easier to read.

Using your understanding of typography, help Aoife Conleavy improve the readability of her site for her readers.

## Finished Website

![image](https://github.com/abemsq/davies-burger-website/blob/master/image.png)

## HTML
```
<!DOCTYPE html>
<html>
<head>
  <title>Davie JR's Menu</title>
  <link href="https://fonts.googleapis.com/css?family=Roboto:100,500,700|Oswald:300,400,700" rel="stylesheet">
  <link rel="stylesheet" type="text/css" href="reset.css">
  <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>

  <!-- Navigation Section -->

  <nav>
    <img src="https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" />
    <span><a href="#">MENU</a></span>
    <span><a href="#">NUTRITION</a></span>
    <span><a href="#">ORDER</a></span>
    <span><a href="#">LOCATIONS</a></span>
  </nav>

  <!-- Content Section -->

  <div class="content">

    <!-- Content Header -->
    
    <div class="header">
      <h1>BBQ BACON BURGER</h1>
    </div>

    <!-- Content Body -->

    <div class="body">
      <p>
        Our BBQ Bacon Burger features our special house ground blend of wagyu and sirloin, spiced perfectly, and finished off with just a drop of white truffle oil. A butter grilled brioche bun layered with roasted red onion, perfectly crispy pork belly, and our hickory smoked BBQ sauce.
      </p>

      <!-- Order Button -->

      <a href="#" class="button">ORDER NOW</a>

      <!-- Nutrition Information -->
      
      <ul class="nutrition">
        <li>
          <span class="category">CALORIES</span>
          <span class="value">678</span>
        </li>
        <li>
          <span class="category">FAT</span>
          <span class="value">32</span>
        </li>
        <li>
          <span class="category">PROTEIN</span>
          <span class="value">8</span>
        </li>
        <li>
          <span class="category">CARBOHYDRATES</span>
          <span class="value">34</span>
        </li>
        <li>
          <span class="category">SODIUM</span>
          <span class="value">112</span>
        </li>
      </ul>
    </div>
  </div>
  
</body>
</html>
```

## CSS
```
/* Universal Styles */

body {
    background-image: url("https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_foodlogo.png");
    text-align: center;
    font-family: 'Roboto', sans-serif;
    font-size: 18px;
  }
  
  a {
    text-decoration: none;
  }
  
  /* Navigation */
  
  nav {
    text-align: center;
  }
  
  nav img {
    display: block;
    width: 180px;
    margin: 0 auto;
  }
  
  nav span {
    display: block;
    font-size: 16px;
    font-weight: 100;
    letter-spacing: 2px;
    margin: 10px 0;
  }
  
  nav a {
    color: #666666;
  }
  
  /* Content Container */
  
  .content {
    width: 100%;
    height: 500px;
    margin: 10px auto;
    overflow: scroll;
  }
  
  /* Content Header */
  
  .header {
    background-image: url("https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_burgerphoto.jpeg");
    background-position: center;
    background-size: cover;
    height: 320px;
  }
  
  .header h1 {
    background-color: #05A8AA;
    color: #FFF;
    font-family: 'Oswald', sans-serif;
    font-size: 40px;
    font-weight: 300;
    line-height: 40px;
    width: 68%;
    padding: 20px;
    margin: 0 auto;
  }
  
  /* Content Body */
  
  .content .body {
    width: 90%;
    margin: 0 auto;
  }
  
  .body p {
    color: #333333;
    font-weight: 100;
    line-height: 34px;
    width: 90%;
    margin-top: 18px;
  }
  
  /* Content Button */
  
  .button {
    border-radius: 4px;
    color: #05A8AA;
    display: block;
    font-weight: 700;
    width: 200px;
    padding: 20px;
    margin: 40px auto;
    border: 1px solid blue;
  }
  
  .button:hover {
    background-color: #05A8AA;
    border: 1px solid #05A8AA;
    color: #FFF;
  }
  
  /* Content Nutrition */
  
  ul.nutrition {
    padding: 20px;
  }
  
  ul.nutrition li {
    display: inline-block;
    background-color: #05A8AA;
    list-style: none;
    width: 200px;
    padding: 0 20px;
  }
  
  .nutrition .category {
    color: white;
    font-weight: 100;
    letter-spacing: 2px;
    display: block;
    margin-bottom: 3px;
  }
  
  .nutrition .value {
    color: white;
    font-size: 26px;
    font-weight: 700;
    letter-spacing: 2px;
  }
```
