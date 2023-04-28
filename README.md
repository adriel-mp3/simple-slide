<h1 align="center">Simple Slide</h1>

<img src="./.github/screenshot1.jpg">

<h2>
  Resume
</h2>

<p>
  The project is a responsive slide that works on different devices such as mobile phones, computers, and 
  laptops. It was developed <b>100% in JavaScript</b>, using classes and the latest modern features of the language.
</p>

<h2>
  Code
</h2>

<p>
  The development in JavaScript allowed for the creation of efficient and robust code, ensuring fast performance and 
  easier and more organized maintenance. Classes were used to structure and organize the code, making it more readable and modular.
</p>

<h2>
  Responsiveness
</h2>

<p>
 In this project, special attention was given to mobile users by adding touch events and preventing possible resize patterns that 
 were causing a lot of bugs. This ensures that the slide is fully responsive and provides a seamless experience for users on different 
 devices, including mobile phones. By incorporating touch events, the slide is optimized for mobile users, who can easily 
 swipe through the slide without any issues. Additionally, by addressing the resize bugs, the project has become more stable and 
 reliable, ensuring a smooth experience for all users.
</p>

<h2>
  How to use
</h2>

<p>
  You should follow this HTML structure to build your slides, pay attention to the classes of the tags that we will pass to the 
  JavaScript class that receives the wrapper and the slide.
</p>

<pre>
  &lt;div class="slide-wrapper"&gt;
    &lt;ul class="slide"&gt;
      &lt;li&gt;&lt;img src="./img/foto1.jpg" alt=""&gt;&lt;/li&gt;
      &lt;li&gt;&lt;img src="./img/foto2.jpg" alt=""&gt;&lt;/li&gt;
      &lt;li&gt;&lt;img src="./img/foto3.jpg" alt=""&gt;&lt;/li&gt;
      &lt;li&gt;&lt;img src="./img/foto4.jpg" alt=""&gt;&lt;/li&gt;
      &lt;li&gt;&lt;img src="./img/foto5.jpg" alt=""&gt;&lt;/li&gt;
      &lt;li&gt;&lt;img src="./img/foto6.jpg" alt=""&gt;&lt;/li&gt;
    &lt;/ul&gt;
  &lt;/div&gt;
</pre>

<p>
  The style.css  file is essential for applying the standard styles of the slide and ensuring its functionality.  It's important to 
  note that the CSS file is available in my GitHub repository, allowing anyone to easily access and use it to enhance their slides.
</p>

<p>
  To use the slide in a website, first import the Slide class from the JavaScript file. Then create a new instance of the Slide class 
  by passing the CSS selectors for the slide container and its wrapper element as arguments. 
  <br>
  <br>
  For example:
</p>

```
import { Slide } from './slide.js';

const slide = new Slide('.slide', '.slide-wrapper');
slide.init();
```

<p>
  The <code>init()</code> method initializes the slide by adding all necessary event listeners and configuring the slide's initial state. The slide 
  will now be functional and ready for use on the website.
</p>

<p>
  There is also the possibility of configuring two different types of navigation from the SlideNav class.
</p>

<h3>
  Navigation by arrow or by simple pagination.
</h3>

<p>
  If you just want to add a simple navigation, just use
</p>

<code>slide.addControl('your class here (optional)')</code>

<p>
  If you want to customize it, just add the class of the element that will be added to the navigation properties.
</p>

To navigate by arrow, just add the method

<code>addArrow('.prev', '.next')</code>

<p>
  And pass the respective classes of each element to be selected by the DOM.
</p> 
