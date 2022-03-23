Page1:

1. ```html
   <ul>
       <li>The Classic - Timeless bouquets for any occasion or décor. We’ll wow you with every single bouquet!
       </li>
       <li>The Seasonal - A farm fresh selection of seasonal flowers. These are sure to brighten any space.
       </li>
       <li>The Luxury - Our Luxury Flowers Include, Hydrangeas, Roses, Calla lilies, peony, etc. Sure to amaze!
       </li>
   </ul>
   ```

   We created an unordered list to showcase the characteristics of our florist and the wide variety of flowers.



2. ```html
   <div class="panel active"
       style="background-image: url(https://images.unsplash.com/photo-1587316830148-c9b01df2da38?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxleHBsb3JlLWZlZWR8MXx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=60);">
       <h3>Tulips</h3>
   </div>
   
   <div class="panel"
       style="background-image: url(https://images.unsplash.com/photo-1591533985237-e813a3f3ebb9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Nnx8ZGFpc2llc3xlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60);">
       <h3>Daisies</h3>
   </div>
   ```

   Here, we referred to the Expanding Cards project in udemy and selected 5 beautiful pictures of flowers as the main part of our home page.



3. ```html
   <nav>
     <ul>
     	<li><i class="fas fa-home"></i><a href="../Page1/page1.html"> Home</a></li>
       <li><i class="fas fa-user-alt"></i><a href="../Page2/page2.html"> Flowers</a></li>
       <li><i class="fas fa-envelope"></i><a href="../Page3/page3.html"> Contact</a></li>
     </ul>
   </nav>
   ```

   Here, we use nav and unordered list elements to achieve mutual access between the three web pages.



4. ```html
   <div class="circle-container">
       <div class="circle">
           <button id="close">
               <i class="fas fa-times"></i>
           </button>
           <button id="open">
               <i class="fas fa-bars"></i>
           </button>
       </div>
   </div>
   ```

   We also referred to the Expanding Cards project in udemy for this part of the code, which creates two buttons that enable the user to open and close the sidebar/nav bar.



5. ```css
   nav a{
       color: rgb(12, 233, 203);
       text-decoration: none;
       transition: all 0.5s;
   }
     
   nav a:hover {
       color: #FF7979;
       font-weight: bold;
   }
   ```

   This part of the code sets the color of the three icons and text in the nav bar when they are stationary, and the color and font-weight that will change when we hover over them. At the same time, we also set the time when that change occurs.



6. ```css
   .panel h3 {
     font-size: 24px;
     position: absolute;
     bottom: 20px;
     left: 20px;
     margin: 0;
     opacity: 0;
   }
   ```

   We changed the font size of the flower names in Expanding Cards and where they appear. In addition, we set these names to be completely transparent, in order to have only active cards display the name.



7. ```css
   .panel.active h3 {
     opacity: 1;
     transition: opacity 0.3s ease-in 0.4s;
   }
   ```

   This part can be understood as an extension of the previous point, where we set the active h3 (the flower name) to be fully visible and implement the transition change and the time required between transparent and visible.



8. ```css
   .circle-container {
       position: fixed;
       top: -100px;
       left: -100px;
   }
   ```

   This part of the code is interesting in that we set the background of the open and close icons in page one to a fixed position in the upper left corner so that the background does not shift as the nav bar expands. In addition, we set both left and top to -100px, so that we get a quarter circle.



9. ```javascript
   open.addEventListener('click', () => container.classList.add('show-nav'))
   close.addEventListener('click', () => container.classList.remove('show-nav'))
   ```

   This part of the js code is very straightforward, it implements the response when we click the open and close icons and the corresponding css effects.



10. ```javascript
    panels.forEach(panel => {
        panel.addEventListener('click', () => {
            removeActiveClasses()
            panel.classList.add('active')
        })
    })
    ```

    Similarly, it implements that when we click on an image in Expanding Cards, the image will be set to active and a series of css changes owned by active.





------

Page2:

1. ```html
   <style>
       body {
           background-color: powderblue;
       }
   
       h1 {
           color: blue;
       }
   
       h2 {
           color: red;
       }
   </style>
   ```

   These code set the value of background-color, h1 and h2. 

   

2. 

   ```javascript
   const search = document.querySelector('.search')
   const btn = document.querySelector('.btn')
   const input = document.querySelector('.input')
   btn.addEventListener('click', () => {
   search.classList.toggle('active')
   input.focus()
   })
   ```

   Those code can help us achieve hidden-search . If customers know what they want. It will be easy way for them.

   

3. 

   ```html
   <ul>
       <li><i class="fas fa-home"></i><a href="../Page1/page1.html"> Home</a></li>
       <li><i class="fas fa-user-alt"></i><a href="../Page2/page2.html"> Flowers</a></li>
       <li><i class="fas fa-envelope"></i><a href="../Page3/page3.html"> Contact</a></li>
   </ul>
   ```

   Those code can help us go to another pager so that it will be easy for us to see different pager .

   

4. 

   ```html
   <ul>
       <li>Roses</li>
       <li>Orchids</li>
       <li>Carnations</li>
       <li>Lilies</li>
       <li>Chrysanthemums</li>
   </ul>
   ```

   Also ,in another point , we use list<ul> and <li> to make it looks more clean.

   

5. 

   ```html
   <img src="https://cdn.shopify.com/s/files/1/0507/3754/5401/t/1/assets/CGYD_LOL_preset_ftd-mx-hero-lv-new.jpeg?v=1647471160"
                       width="20%" alt="Hello Sunshine Bouquet">
   ```

   In this project ,we use some picture so that we use "width" to make same size for each pictures , using "src" to get picture and use "alt" to name each pictures.

   

6. ```html
   <div>
       <h2>What are the best romantic flowers?</h2>
       <p>If youre looking to send romantic flowers, we have the resources to let you know which are the best
           blooms
           to
           send to your romantic partner. Just some of the most romantic blooms include favorites like:</p>
       <ul>
           <li>Roses</li>
           <li>Peonies</li>
           <li>Tulips</li>
           <li>Carnations</li>
           <li>Irises</li>
           <li>Sunflowers</li>
       </ul>
   </div>
   ```

   In this project , i use a lot of <div> because it can help me better plan every part.

   

7. 

   ```html
   <h1 id="QA_h1">Best Selling Flowers Frequently Asked Questions</h1>
   <h2>What are the best selling flowers?</h2>
   ```

   Also , i used <h1> and <h2> .It can make the hierarchical relationship of the page clearer and allow search engines to better crawl and analyze the subject content of the page.

   

8. 

   ```html
   <p>Picking the best flowers to have delivered for your special occasion depends on a variety of factors, including what message you want them to relay, why you're sending them, and how long you want them to last. That said,some of our top-selling flowers year-round include:</p>
   ```

   Our goal is about selling our products so I use <p> to explain every single product we have.

   

9. 

   ```css
    background-color: #fff;
    border: 0;
    font-size: 18px;
    padding: 15px;
    height: 50px;
    width: 50px;
    transition: width 0.3s ease;
   ```

   We have a lot of things in one pager so we need to set border , padding , height and so on for different elements.

   

10. 

    ```html
    <img src="https://static-resources.zybooks.com/star.png" alt="star">
    <img src="https://static-resources.zybooks.com/star.png" alt="star">
    <img src="https://static-resources.zybooks.com/star.png" alt="star">
    <img src="https://static-resources.zybooks.com/star.png" alt="star">
    ```

    This is how we advise our guests.





------

Page3:

1. ```html
   <form id="info" method="post">
       <div class="formgroup" id="name-form">
           <label for="name">Your name*</label>
           <input type="text" id="name" name="name" />
       </div>
   
       <div class="formgroup" id="email-form">
           <label for="email">Your e-mail*</label>
           <input type="email" id="email" name="email" />
       </div>
   
       <div class="formgroup" id="message-form">
           <label for="message">Your message</label>
           <textarea id="message" name="message"></textarea>
       </div>
   ```

   Here, we create a form for the user to provide their name, email, and a textbox to fill out with specific content.



2. ```html
   <table style="width:100%">
       <tr>
           <th>branch</th>
           <th>Contact</th>
           <th>City</th>
       </tr>
       <tr>
           <td>Art Flower（Flushing Flower)</td>
           <td>heteng</td>
           <td>NY</td>
       </tr>
       <tr>
           <td>Centro comercial Moctezuma</td>
           <td>Chang</td>
           <td>NJ</td>
       </tr>
   </table>
   ```

   Here, we created a very simple table that contains the name and location of our branch and the name of our contact.



3. ```css
   h1{
   	font-weight: normal;
   	font-size: 4em;
   	margin:335px auto;
   	width: 500px;
   	color: #F90;
   	text-align: center;
   }
   ```

   This part of the code is very straightforward, it sets the font-size, font-weight, color, position and other basic css properties of h1 (aka "Contact us") of our page 3.



4. ```css
   input:focus, textarea:focus{
   	border: solid 3px #77bde0;	
   }
   ```

   The css code sets the values of border-width, border-style, and border-color in input and texteara to be solid 3px #77bde0.



5. ```css
   input[type="submit"]{
   	background-color: #e58f0e;
   	color: white;
   	height: 50px;
   	cursor: pointer;
   	margin-top: 30px;
   	font-size: 1.29em;
   }
   
   input[type="submit"]:hover{
   	background-color: #e9e50c;	
   }
   ```

   Here, we set the background color of the submit button, the font size and a series of basic css properties. In addition, we also set the color change that occurs when the cursor hovers over the button.



6. ```css
   .bg {
       background: url('https://images.unsplash.com/photo-1647601160679-b22ac0f22d73?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwxMjB8fHxlbnwwfHx8fA%3D%3D&auto=format&fit=crop&w=500&q=60'); 
       position: absolute;
       top: -30px;
       left: -30px;
       width: calc(100vw + 60px);
       height: calc(100vh + 60px);
       z-index: -1;
       filter: blur(0px);
    }
   ```

   This part of the code contains a lot of things, but in terms of focus, we use an image of a flower as the background that appears when entering page 3. The interesting thing is that when setting the values of width and height, we use a calc, in order to reduce the white space around the edges in the blurred state.



7. ```css
   input, textarea{
   	width: 500px;	
   	border: none;
   	border-radius: 20px;
   	outline: none;
   	padding: 10px;
   	font-family: 'Lato', sans-serif;
   	font-size: 1em;
   	color: #676767;
   	transition: border 0.5s;
   	border: solid 3px #98d4f3;	
   	box-sizing:border-box;	
   }
   ```

   Again, this section uses a lot of css properties. In short, we standardize the size, padding and other properties of input, textarea element. It is worth mentioning that we set border-radius to 20px to give rounded corners around the text box and reduce the overall sharpness.



8. ```javascript
   let int = setInterval(blurring, 30)
   ```

   We created a variable here to run a function called blurring every 30 milliseconds since we don't want it run very slow.



9. ```javascript
   function blurring() {
       load++
   
       if (load > 99) {
           clearInterval(int)
       }
   
       loadText.innerText = `${load}%`
       loadText.style.opacity = scale(load, 0, 100, 1, 0)
       bg.style.filter = `blur(${scale(load, 0, 100, 30, 0)}px)`
   }
   ```

   This is the core part of javascript in page3, which realizes the process of 0% ~ 99% and the change of the whole page background from blurred to clear.



10. ```css
    @import url('https://fonts.googleapis.com/css?family=Muli&display=swap');
    ```

    We use the @import rule to import external fonts in CSS, we get the link to the font we want from "Google Fonts" and put it in the url() function.