# EngineerHamziey's **EXPLAINED** Solution To Frontend Mentor - Stats preview card component :relieved:.
:relieved:*Trust me, we are going to have fun and learn at the same time, I'll make this as interesting as possible*:wink: :yum:
## Table of contents
  
  - [Acknowledgments](#acknowledgments)
  - [My Social Media Links](#my-social-media-links)
  - [My Solution](#my-solution)
  - [Picture of what we are building and learning](#screenshots)
  - [Markup/HTML Explanation](#HTML-explanation)
  - [Stylesheet Explanation](#CSS-explanation)
  - [To ask questions on my solution](#links)


## My Social Media links
If you find this helpful, kindly follow me on GitHub or and My other social media below to see more blog/tutorial/content like this :wink:

- My LinkedLn - [Lawal Hamzat Ademola](https://www.linkedin.com/in/hamzat-lawal-a88404239)
- My Frontend Mentor - [@EngineerHamziey](https://www.frontendmentor.io/profile/EngineerHamziey)
- My Twitter: [@EngineerHamziey](https://twitter.com/EngineerHamziey?t=CTYHt_bIgYlMNIE6IM5dSw&s=09)
- You can hire me on Upwork for your frontend web projects: [Engineer Lawal Hamzat Ademola](https://www.upwork.com/freelancers/~012d93ee2163d44605)


## Acknowledgments
:blush:I would like to express my special thanks to @jamesqquick for finally inspiring me to do this(Teach as I learn). 
Also special Thanks to Vanza Setia, Grace Snow and all other Mentors on [Frontend Mentor](https://www.Frontendmentor.io) for corrections, recommendations and suggestions on my solutions, I love you guys:kissing_closed_eyes:.



### My Solution
This is my solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62) with explanation by me [EngineerHamziey](https://www.linkedin.com/in/hamzat-lawal-a88404239). The code contains comments that explains how and why I am doing things, and you can also find the eplanation below on this ReadMe page. My aim is to help others Learn What I have Learnt so feel free to ask questions(or make recommendations), star or fork this repository, you can also follow me on GitHub to Know when there is a new tutorial. If you have any contribution, question or observation, you can reach me out to me by commenting here( [Twitter](d) [Linkedln](d) [Frontend-mentor](d)). Those are the links to this tutorial post where we can have discussion.



Users should be able to:
- View the optimal layout depending on their device's screen size(i.e this should be responsive) and it should be fairly accessible(as I am just starting learn accessibility)
- I built the Solution Using HTML, CSS and JavaScript.
## Screenshots
![](./images/my-statsScreenshot.png)
![](./design/mobile-design.jpg)


### Links

- [Code URL](https://github.com/EngineerHamziey/stats-preview-card-component-main)
- [Live Site URL](https://hamzat-stats-preview.netlify.app)
- [Solution Page On Frontend Mentor](https://www.frontendmentor.io/solutions/stats-preview-card-with-full-explanation-using-flexbox-and-mobile-fi-TzujRpTkxz)

### Built with

- Semantic HTML5 markup(Enabling Good Accessibity To Help Assistive Technology Users )
- CSS custom properties
- Flexbox
- Mobile-first workflow


## HTML Explanation 
:blush:*let's dive right in*:kissing_heart:

---

we start by declaring the `<!DOCTYPE html>` html here implies html 5

---
then we tell the language globally using the "lang" attribute `<html lang="en"` "en" here means english. Always put the lang attribute, to help assistive technologies(avoid accessibility issues).

---

 always set your charset to UTF-8 (or whatever you intend to use)first after the head tag
 `<meta charset="UTF-8">`

 ---

`<meta name="viewport" content="width=device-width, initial-scale=1.0">` these makes the site display properly based on user's device width and an initial scale of 1 means with neither zoom-in nor zoom-out. Hope you're getting it? :simple_smile:

 ---

 `<meta name="Keywords" content="EngineerHamziey, Frontend Web Developer">` this is for SEO(You can ignore it for now or check MDN web doc if you're curious).

 ---

 ---

 `<link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">` this is simply used to link the icon that appears beside the title of the webpage.

 ---

 `<link rel="stylesheet" href="./styles/mobile.css">` This simply links to our stylesheet( as you would expect:smiley:)

 ---

 ---

 `<title>EngineerHamziey's Solution To Stats preview card component</title>` here is the title of our webpage

 ---


:relaxed: so far we have this :
```html
<!DOCTYPE html>
<html lang="en">
  <head>
  <meta name="description"
    content="This is Engineer Hamzieys Solution To Frontend Mentor stats preview card component challenge">
  <meta name="Keywords" content="EngineerHamziey, Frontend Web Developer">
  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <link rel="stylesheet" href="./styles/mobile.css">
  <title>EngineerHamziey's Solution To Stats preview card component</title>
</head>
.
.
.

```

### What we have next is the body, in our Body, we have :


```html
.
.
.
<body>
  <!-- yh, Always put your Web content in a landmark element(!important for accessibility purpose).
  Examples of landmark elements include: main, footer, header,section, aside, etc.
  The main is expected to contain the main part of the page just like its name suggest,
  remember NOT TO PUT ONE LANDMARK IN THE OTHER -->
  <main class="main-container">
   
    <div class="the-img">
       <!--
      I want to add the image as background image to this div.the-img, its a decorative image and we don't need to add alt text for assitive technology users 
    -->
    </div>

    <!-- I'm putting the text in  this div.typography -->
    <!-- in general, I grouped the texts in containers so that I can position them together -->
    <div class="typography">
      <div class="top-text">
        <!-- I wrapped the word "insights" in a span with class emphasized so that I can changed its color in my css -->
        <h1>Get <span class="emphasized">insights</span> that help your business grow.</h1>
        <p>
          Discover the benefits of data analytics and make better decisions regarding revenue, customer
          experience,
          and
          overall efficiency
        </p>
      </div>
      <!-- 
        making this a list item is better to make it semantics
        cuz if you think of this without styling, it's just a list.
              -10k+ companies
              -314 templates
              -12m+ queries
       -->
      <ul class="stats">
        <li>
          <!-- we don't need to use heading here since this ain't a title, it's just a big text ""
          we can use the strong tag <strong> or p, then we style it with our CSS -->
          <p class="number">
            10k+
          </p>
          <p class="rating">
            <!--
              let's write this as small letter first, then
              use our CSS(text-transform) to turn it to uppercase so that the screenreaders
              will read it out as a word and not letter by letter like an abbrevation or something
            -->
            companies
          </p>
        </li>
        <li>
          <p class="number">
            314
          </p>
          <p class="rating">
            templates
          </p>
        </li>
        <li>
          <p class="number">
            12M+
          </p>
          <p class="rating">
            queries
          </p>
        </li>
      </ul>
    </div>

  </main>


  <!-- Always place your web content in a landmark element. The  footer is the best landmark here to make it( accessible). -->
  <footer>
    <div class="attribution">
      <p>
        Challenge by
        <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. Coded by <a
          href="https://www.linkedin.com/in/hamzat-lawal-a88404239">Lawal Hamat Ademola</a>. <a
          href="https://github.com/EngineerHamziey/stats-preview-card-component-main.git">Code Link on github.</a>
      </p>
      <p>To see Menthors' feedback on the code,
        <a href="#">Click here.</a>
      </p>
    </div>
  </footer>
</body>

<!-- congratulations, we just finish the writing the mark-up -->
</html>
```
Now lers move to the styling :relieved: , at this juncture, if you have any question jot so that you can ask it all at once on the [comment](#links).



## CSS Explanation 
*We will be designing for mobile layout first, because it often lead to an efficient and shorter code and mobile users won't have to process all of the desktop styles.*
```CSS
/* let's import our font(you can google search "how to link google fonts in my css, if you're unfamiliar with it") */
@import url('https://fonts.googleapis.com/css2?family=Lexend+Deca:wght@400;700&display=swap');


/*
  Storing some properties like color, max-width, etc in a variable is a good idea and makes
  your work fast as you can easily type in the variable name without trying to remember
  the rgb or hex value of a color. It ALso makes it easy to change values of all occurence of the property
  the :root is the best place to declare the variable to make it global(that is, so that you can access it anywhere in your code)
*/

:root {
  /* 
    the syntax for variable declaration is simple, just start with double dash "--" as shown below, you
    since the name is more than a word, I seperated them with a dash, you can use camel case or Pascal case as well
  */

  /* main background colour*/
  --Very-dark-blue: hsl(233, 47%, 7%);
  /*  card background colour*/
  --Dark-desaturated-blue: hsl(244, 38%, 16%);
  /* accent */
  --Soft-violet: hsl(277, 64%, 61%);
  /* main heading and stats */
  --White: hsl(0, 0%, 100%);
  /* main paragraph */
  --main-paragraph: hsla(0, 0%, 100%, 0.75);
  /* stat headings */
  --Stats-headings: hsla(0, 0%, 100%, 0.6);
/* the overlay */
  --overlay: rgba(128, 10, 197, 0.5);
}

/* let's remove the default padding and margin for every object on
the page to ensure that all margin and padding are intentional */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Now the journey begins, smile */
body {
  /*
    Use a minimum value of 1.5 for line-height for main paragraph content. This will help people experiencing low vision conditions(accessibility things),
    as well as people with cognitive concerns such as Dyslexia. If the page is zoomed to increase the text size, using a unitless value
    ensures that the line height will scale proportionately.,
    --line-height is used to define the minimal height of line boxes within the element. It allows you to set the height of a line
    independently from the font-size it sets the differences between two lines of your content.It defines the amount of spaces
    above or below inline elements.
    --THE DEFAULT IS VALUE of line-height IS 1
    TO LEARN MORE ABOUT THIS >> https://developer.mozilla.org/en-US/docs/Web/CSS/line-height#accessibility_concerns
  */
  line-height: 1.5;

  background: var(--Very-dark-blue);
  /* 
    inorder to center the page vertically and horizontally,
    you should use flexbox. For that you will need to add min-height 100vh to the body to ensure that it takes up the minimum height of 100vh
    min-height is the best option so that will grow bigger when needed(i.e responsive). min-height NOT HEIGHT, using ordinary height, won't 
    allow responsiveness (it will make the code looked)
  */
  min-height: 100vh;
  /* then we can now center it with flexbox */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* using rem instead of px is a good idea for responsiveness */
  /* converting 15px to rem : 15px/16px = 0.9375rem, since 15px is recommended in the style guild */
  font-size: 0.9375rem;
  font-family: "Lexend Deca",sans-serif;
  /* let's put some padding here so that all the content of the whole page won't get cut off by the edge of the browser,
  you can actually use margin on the card instead*/
  padding: 1rem 0.7rem;

  /*since every text is align at the center on the mobile design and we're building mobile first,
  I'll set the text-align property of my body to center intead of doing it for all individually */
  text-align: center;
}

.main-container {
  /* now, here is how you call your variable and auto-completion/auto-suggestion will help you out */
  background: var(--Dark-desaturated-blue);
  /*
   let's put some margin so that the card is further away from the edges of the browser, i.e so that it won't be too close to or cut-off by the edge or the corner of the browser
   */
  
  /* margin: y-Axis x-Axis; y-axis(top and bottom) x-axis(top and bottom) */
  margin: 2rem 0.5rem;
  /* max-width here is extremely important so that the card(main) won't grow too wide on wide screens like tab in this 
  case since this is our mobile version and we are not designing for tab and max-width should be placed on the card, NOT the body*/
  max-width: 23rem;
  /* to give it round corner */
  border-radius: 0.9rem;
  /* let's set the overflow to hidden so that the sharp corner of the image won't pop out of the card */
  overflow: hidden;
}

/* the img */
.the-img {
  /* 
    I don't how to explain these background image in few words, I'll suggest visiting the link below for more explanation
    for how to add overlay using linear-gradient: https://www.geeksforgeeks.org/css-combine-background-image-with-gradient-overlay/
    for more on how to use background image: https://www.w3schools.com/cssref/pr_background-image.asp
    there are also atleast two other methods out there
  */
  background: linear-gradient(var(--overlay), var(--overlay)),
  url(../images/image-header-mobile.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  /* although all this background... can be done using just a line, but I prefer to show the property name  */

  /* seting the height alone is ok for the mobile version, the width will automatically take up 100% */
  height: 15rem;
}

.typography {
  /*adding padding to the overall text container*/
  padding: 1rem;
}

/* the typography part, haha */

.top-text h1 {
  color: var(--White);
  /* padding: y-axis x-axis; */
  padding: 1.5rem 1rem; 
  font-size: 1.8rem;
}

.emphasized {
  color: var(--Soft-violet);
}

.top-text p {
  color: var(--main-paragraph);
  margin: 1rem;
}

.stats {
  /* remove the default list styling and add some margin */
  list-style: none;
  margin-top: 2rem;
}

li {
  margin: 1.5rem;
  /* transform the text to uppercase,*/
  text-transform: uppercase;
  /*  
      we wrote this as small letters first, then
      use our CSS to turn it to uppercase so that the screenreaders
      will read it out as a word and not letter by letter like an abbrevation (or accronym) 
  */
}

.number {
  color: var(--White);
  /* setting the font sizes looks like eye/vision test for me, I hope this 1.4rem matches it (lol) */
  font-size: 1.4rem;
  /* make the number bold too */
  font-weight: bold;
  margin: 0.2rem;
}

.rating {
  color: var(--Stats-headings);
}


/* here comes the footer */
.attribution {
  margin-bottom: 1.5rem;
  /* converting the given 11px to rem, 11px/16px = 0.6875rem,  */
  font-size: 0.6875rem;
  text-align: center;
  color: #fff;
}

.attribution a {
  color: var(--Soft-violet);
}

.attribution p:nth-child(2) {
  margin-top: 0.3rem;
}

/* 
  :focus-visible 
  An outline is a line that is drawn just outside the boder edge of the elements. Outlines are generally used to indicate focus or active states
  of the elements such as buttons, links, form fields, etc.   
*/
a:focus-visible {
  outline: 0.1rem dotted #f4f4f4;
}


/* when viewd with my chrome dev tools(using dimensions: responsive), the desktop looks good until about 780px, so I used min-width 785px,
which means, the minimum screensize for the desktop styling to kick in is 785px  */
@media (min-width: 785px) {
  
  body {
    /* let's change the text-align to default i.e just unset it since everything isn't align at the center like it was on the mobile design*/
    text-align: unset;
  }

  .main-container {
    /* the margin is obviously used to make space between the card and edge of the browser esspecial on smaller sceens where the card tends to go into the edge of the edge of the browser  */
    margin: 2rem 1rem;
    /* arranging the image and the typoraphy side by side, as opposed to the vertical position on mobile version using flex-box */
    display: flex;
    flex-direction: row-reverse;
    /* giving it a max-width so that it won't too wide on wider screens and it will shrink down when needed(on smaller screens), using JUST width: 90rem; here will cause reponsiveness PROBLEM, as it will make
    make the width fixed(i.e non-reponsive) unlike using max-width. */
    max-width: 90rem;
  }

  .the-img {
    /* let's repeat the same thing as in the mobile background, just changing the image url to the desktop background image */
    background: linear-gradient(var(--overlay), var(--overlay)),
    url(../images/image-header-desktop.jpg);
    /* background-size and background-repeat has been set to cover and no-repeat respectively on the mobile version, so no need to repeat that */

    /* unset here cancells out the previous height we set in our mobile version, just like it's name suggest */
    height: unset;
    /* <!-- we need to give it width here since we want to share the entire screen width between two things --> */
    min-width: 50%;
  }

  .typography {
    /* adding more space around the texts in general*/
    padding: 2rem;
    /* I intentionally put this amount of margin to Ensure that the stats/ratings still have a little space between them on small screen of about 
    769px without additional media query */
  }

  .stats {
    /* making the stats/rating horizontal */
    display: flex;
  }

  .number {
    /* some margin */
    margin: 0.5rem 0;
  }

  ul {
    /* padding: top right bottom left;
    to master this, just remember that the first one is the top, then go in the clockwise direction to right, then bottom and finally left */
    padding: 0 0.5rem 1.5rem 1rem;
  }

  li {
    /* adding auto margin to the right of each stat and removing the others */
    margin: 0 auto 0 0;
  }



}

``` 


## DISCLAIMER:

- some of the things I did(like amount of padding in some places) in this code are due to my personal belive/like
  like storing those colors in a variable, someone might feel it's not necessary since   this is a small project.

- some explanation here might look unnecessary but I put it there because I have seen alot of people make those mistakes

- hopefully, I'll try as much as possible to update the code with corrections and more suggestions,
    but I'll advise that you visit the solution page to see the suggestions and hopefully corrections in the comment section




## RECOMMENDATIONS:
- you can skip some explanation if they are things you understand already.

- some things(like some margins and paddings) are not explained, because I think what they do is simple.
  But if you don't get it, feel free to google it, experiment with it by changing the values and ask questions in the [comment](#links)

- If you don't know much about how to test responsiveness, simply google "how to test responsiveness using chrome developer tool" 

- Also most of the times you don't need to set height for things like this card to ensure responsiveness and so that your
media qery wont look like rocket science :laughing: I mean so that it won't be unnecessarily complex.:wink:

- always use rem, em, %, vh and vw for responsiveness, *ALTHOUGH* using vh and vw sometimes might be a bad idea :sweat: For example, when setting the height or width of the a web component (like a card or something) on the page should not use vh nor vw, because of ultra small screen and ultra wide screen(it is most likesly gonna look ugly on mobile landscape mode, you can experiment with it).
this might look good on your computer, but remember there are many computers out there width smaller and bigger screen size and it will
look good on few BUT BAD ON MOST. As you can see, I used rem for the max-width of the card.



