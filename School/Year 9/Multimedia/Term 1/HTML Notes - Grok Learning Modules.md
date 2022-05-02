# HTML notes
#School 

HTML stands for Hypertext Markup Language, and CSS is Cascading Style Sheets

btw, i don’t bother tidying up my HTML

you need to declare <!DOCTYPE HTML> when starting your HTML.

```html
   <!DOCTYPE HTML>
```

-   Cheat sheet “Hello, World!”
    
    ```html
    <!DOCTYPE HTML>
    <html>
      <h1>Hello, World!</h1>
    </html>
    ```
    

You need to end your blocks with </text> but replace text with what you’re trying to close.

```html
<h1>This is a heading</h1>
```

Headings go from <h1> to <h6>, the number being the size(h1 is largest etc)

```html
<h1>This is the largest heading that you can get</h1>
<h2>This is the second largest heading</h2>
<h3>This is the third largest heading</h3>
<h4>This is the third smallest heading<h4>
<h5>This is the second smallest heading<h5>
<h6>This is the smallest heading<h6>  
```

Paragraphs are just <p>

```html
<p>Your paragraph goes here</p>
```

-   Cheat sheet “Argleton”
    
    ```html
    <!DOCTYPE HTML>
    <h1>Argleton</h1>
    
    <p>Argleton was a phantom settlement that appeared on Google Maps but does not actually exist. The supposed location of Argleton was within the civil parish of Aughton in West Lancashire, England, which in reality is nothing more than empty fields.</p>
    
    <p>Data from Google are used by other online information services which consequently treated Argleton as a real settlement. As a result, Argleton also appeared in numerous listings for things such as real estate, employment and weather.</p>
    
    <h2>Media interest</h2>
    
    <p>The anomaly was first noticed by Mike Nolan, head of web services at nearby Edge Hill University, who posted about it on his blog in September 2008. The story was later picked up by the local media and By November 2009, news of the non-existent town had received global media attention, and "Argleton" became a popular hashtag on Twitter.</p>
    
    <h2>Explanations</h2>
    
    <p>One possible explanation for the presence of Argleton is that it was added deliberately as a copyright trap, or "paper town" as they are sometimes known, to catch any violations of copyright.</p>
    
    <p>Alternatively, it has been suggested that "Argleton" is merely a misspelling of "Aughton", although both names appear on the map. Professor Danny Dorling, president of the Society of Cartographers, considered it more likely that Argleton was nothing more than an "innocent mistake".</p>
    ```
    

You can add colours to the paragraphs or heading by using

```html
<h1 style=”color: lightblue”>insert your text here</h1>
```

You can save time by using consistent styled CSS by putting the tags

```html
<!DOCTYPE html>
<style>
  h1 {
     color: lightblue;
  }
</style>
<h1> Hello World!</h1>
<h1> This is a test!</h1>
```

-   Cheat sheet “True Blue”
    
    ```html
    <!DOCTYPE html>
    <html>
    <h1 style="color: powderblue">Powder Blue</h1>
    <h1 style="color: lightblue">Light Blue</h1>
    <h1 style="color: skyblue">Sky Blue</h1>
    <h1 style="color: cornflowerblue">Cornflower Blue</h1>
    <h1 style="color: royalblue">Royal Blue</h1>
    <h1 style="color: blue">Blue</h1>
    <h1 style="color: darkblue">Dark Blue</h1>
    <h1 style="color: midnightblue">Midnight Blue</h1>
    </html>
    ```
    

You can change the typeface of a paragraph, heading. You set it by doing this, but not all browsers support every single font, some are platform specific, like Apple’s San Francisco typeface.

```html
<p style="font-family: '*insert font name*'">Text</p>
```

To overcome this issue, you put in multiple typeface options by doing

```html
<p style="font-family: '*insert font name*', *other font*, *other font*">Text</p>
```

Your average heading is 32pixels, and the body is 16px. You can change this with CSS properties.

```html
<style>
  h1 {
    font-size: 20px;
  }
</style>
<h1>Heading 1</h1>
<p>Paragraph</p>
```

Some people want the lines to be spaced our slightly more, so it is easier for you to read. You can change this through CSS as well.

```html
<style>
  p {
    line-height: 2;
  }
</style>
<p>just a bunch of random text here that goes on for a very long time until it wraps around and starts a completely new paragraph just to demonstrate line spacing correctly, alright this should be long enough of a paragraph to demonstrate</p>
```

You can put margins in HTML so you can space things out better, the width element determines how wide the element is.

```html
<style>
  p {
    margin-left: 40px;
    width: 160px;
    background-color: orange;
  }
</style>
<p>This should be put into a perfect orange box, and no text should get out</p>
```

-   Cheat sheet “Monospacious”
    
    ```html
    <!DOCTYPE html>
    <style>
      h1 {
        margin-top: 30px;
        margin-left: 40px;
        margin-bottom: 30px;
        font-family: Verdana, Geneva, sans-serif;
        font-size: 36px;
      }
      p {
        width: 680px;
        margin-bottom: 30px;
        margin-left: 40px;
        line-height: 1.8;
        font-size: 18px;
        font-family: Georgia, Times, serif;
      }
      span {
        font-family: 'Courier New', monospace;
      }
    </style>
    <h1>Monospaced fonts</h1>
    
    <p>
    In a monospaced font, the letters all occupy the same amount of horizontal space. In variable-width fonts, the size of letters and spacings between them can be different.
    </p>
    
    <p>
    You're editing this paragraph in a code editor with a monospace font, but styling it with a variable-width font! As well as making coding easier, monospace fonts are fun because you can create ASCII art with them. Style the following span with a monospace font and see what happens!
    </p>
    
    <span>
      ........_.......______.....______..____
      _.._____........_..............._......<br>
      ......./.\\.....'.____.\\...'.___..||_...
      _||_..._|....../.\\............./.|_....<br>
      ....../._.\\...|.(___.\\_|/..'...\\_|..|.|
      ....|.|......./._.\\....._..--.`|.|-'...<br>
      ...../.___.\\..._.____`..|.|.........|.|
      ....|.|....../.___.\\...[.`/'`\\]|.|.....<br>
      ..._/./...\\.\\_|.\\____).|\\.`.___.'\\._|.|
      _.._|.|_..._/./...\\.\\_..|.|....|.|,....<br>
      ..|____|.|____|\\______.'.`.____..'|____
      _||_____|.|____|.|____|[___]...\\__/....<br>
    </span>
    ```
    

To bold an area/highlight something you use the <strong> tags and <em> tags for italics. You might know in Markdown(discord formatting) that bold is **text** and italics are _text_

```html
<p>
This is some very <strong>important</strong> text, and this is very <em>interesting</em>

```

You can break up sentences with a simple <br> which stands for break. You **don’t** need to close the code with a </> This is known as a “Self Closing Tag”

```html
<p>
This paragraph is now <br> broken
</p>
<p> This paragraph is not broken <p>
```

-   Cheat sheet “Shakespeare”
    
    ```html
    <!DOCTYPE HTML>
    <p><strong>HELENA:</strong> Ay, do. Persever, counterfeit sad looks,<br>
    Make mouths upon me when I turn my back,<br>
    Wink each at other, hold the sweet jest up-<br>
    This sport, well carried, shall be chronicled.<br>
      <br>
    </p>
    <p>
    If you have any pity, grace, or manners,<br>
    You would not make me such an argument.<br>
    But fare ye well. 'Tis partly my own fault,<br>
    Which death or absence soon shall remedy.
    </p>
    <p><strong>LYSANDER:</strong> Stay, gentle Helena. Hear my excuse.<br>
      My love, my life, my soul, fair Helena!<br></p>
    
    <p><strong>HELENA:</strong> Oh, excellent!</p>
    
    <p><strong>HERMIA <em>(to LYSANDER)</em>:</strong> Sweet, do not scorn her so.</p>
    
    <p><strong>DEMETRIUS:</strong> If she cannot entreat, I can compel.</p>
    
    <p><strong>LYSANDER:</strong> Thou canst compel no more than she entreat.<br>
    Thy threats have no more strength than her weak prayers.-<br>
    Helen, I love thee. By my life, I do.<br>
    I swear by that which I will lose for thee<br>
      To prove him false that says I love thee not.<br></p>
    
    <p><strong>DEMETRIUS:</strong> I say I love thee more than he can do.</p>
    
    <p><strong>LYSANDER:</strong> If thou say so, withdraw and prove it too.</p>
    ```
    

You can center text in HTML. The heading in this example is centered.

```html
<style>
h1 {
    text-align: center;
    width: 600px;
}
p {
    text-align: justify;
    width: 600px;
}
</style>
<h1>Centered Heading</h1>
<p>
This text is justified. Text lines up the left and right edges to the left and right content edges of the paragraph. Justified text is often used in newspapers, although studies have shown that text with jagged edges, that is, non-justified text, is easier to read as the eyes can more easily keep track of one's progress. 
</p>
```

The span element is used to style a small part of text in a paragraph without actually styling the entire paragraph.

```html
<p>
  My favourite colour is <span style="color: red">red</span>.
</p>
<p>
  This <span>span tag</span> has no effect.
</p>
```

You can use RGB colours to set text colours with CSS styling. These colours can be found by searching RGB colour picker in google

```html
<p style="color: rgb(255, 0, 0)">Red</p>
<p style="color: rgb(0, 255, 0)">Green</p>
<p style="color: rgb(0, 0, 255)">Blue</p>
<p style="color: rgb(255, 128, 0)">Orange</p>
<p style="color: rgb(128, 20, 180)">Purple</p>
```

-   Cheat sheet “It’s not easy being green”
    
    ```html
    <!DOCTYPE HTML>
    <html>
      <style>
        h1 {
          text-align: center;
        }
      </style>
      <h1><span style="color: rgb(0, 0, 0)">Kermit</span> <span style="color: rgb(240, 255, 240)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 40, 0)">Kermit</span> <span style="color: rgb(200, 255, 200)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 80, 0)">Kermit</span> <span style="color: rgb(160, 255, 160)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 120, 0)">Kermit</span> <span style="color: rgb(120, 255, 120)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 160, 0)">Kermit</span> <span style="color: rgb(80, 255, 80)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 200, 0)">Kermit</span> <span style="color: rgb(40, 255, 40)">Kermit</span></h1>
      <h1><span style="color: rgb(0, 240, 0)">Kermit</span> <span style="color: rgb(0, 255, 0)">Kermit</span></h1>
    </html>
    ```
    

Links are done by using the href attribute. They are done with <a href=”link”></a>

```html
<p>
<a href="<https://google.com>">Click here</a> to go to google
</p>
```

You can remove text underlining by using the text-decoration: none; flag.

```html
<style>
  a {
    text-decoration: none;
  }
</style>
```

-   Cheat sheet “Linking Wikipedia”
    
    ```html
    <!DOCTYPE html>
    <style>
      p {
        font-size: 14px;
        line-height: 1.6;
        width: 600px;
        margin-left: 20px;
      }
    
      a {
        text-decoration: none;
        color: rgb(6, 69, 173);
      }
    
      h1 {
        font-family: Georgia, Times, serif;
        font-size: 25px;
        line-height: 1.3;
        margin-bottom: -10px;
        margin-top: 20px;
        margin-left: 20px;
        border-bottom: 1px solid darkgray;
        font-weight: normal;
      }
    </style>
    <h1>Tim Berners-Lee</h1>
    <p>From Wikipedia, the free encyclopedia</p>
    <p>
    <strong>Sir Timothy John</strong> "<strong>Tim</strong>" <strong>Berners-Lee</strong>, (born 8 June 1955), also known as <strong>TimBL</strong>, is an English computer scientist, best known as the inventor of the <a href="<https://en.wikipedia.org/wiki/World_Wide_Web>">World Wide Web</a>. He made a proposal for an information management system in March 1989,
     and he implemented the first successful communication between a <a href="<https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol>">Hypertext Transfer Protocol (HTTP)</a> client and server via the Internet sometime around mid-November of that same year.
    </p>
    
    <p>
    Berners-Lee is the director of the <a href="<https://en.wikipedia.org/wiki/World_Wide_Web_Consortium>">World Wide Web Consortium</a>, which oversees the Web's continued development. He is also the founder of the <a href="<https://en.wikipedia.org/wiki/World_Wide_Web_Foundation>">World Wide Web Foundation</a>, and is a senior researcher and holder of the Founders Chair at the <a href="<https://en.wikipedia.org/wiki/MIT_Computer_Science_and_Artificial_Intelligence_Laboratory>">MIT Computer Science and Artificial Intelligence Laboratory</a>.
    </p>
    
    <p>
    In 2004, Berners-Lee was knighted by <a href="<https://en.wikipedia.org/wiki/Elizabeth_II>">Queen Elizabeth II</a> for his pioneering work. He was honoured as the "Inventor of the World Wide Web" during the <a href="<https://en.wikipedia.org/wiki/2012_Summer_Olympics_opening_ceremony>">2012 Summer Olympics opening ceremony</a>.
    </p>
    ```
    

When you set the width of an element, it will stop stretching outside of its container. You can center the element using the auto left/right margins.

```html
<style>
h1 {    
    width: 600px;
    margin-left: auto;
    margin-right: auto; 
    background-color: lightgray;
}
</style>
<h1>
This heading and its grey background show how to centre a specific element, which could be headings or paragraphs.
</h1>
```

You can add images to a website using the img element. (alt is the text that it shows when there is no picture to show)

The img tag is self closing, you don’t need to do </img>

```html
<img src="cat.jpg" alt="A picture of a cat">
```

You can resize your images with the “width” and “height” html tags.

The first one ties the width and the height together and makes it scaled correctly. The second one stretches the image 300 pixels high and 100 pixels wide.

```html
<img src="cat.jpg" alt="A cat" width="100" >
<img src="cat.jpg" alt="A cat" width="100" height="300" >
```

You can specify dimensions. to a percentage of the image. This tag can be set right onto the image tag

```html
<img src="cat.jpg" alt="A cat" style="width:50%">
<img src="cat.jpg" alt="A cat" style="width:100%">
```

-   Cheat sheet “Holiday Blog”
    
    ```html
    <!DOCTYPE html>
    <style>
    p {
      font-size: 20px;
      margin-bottom: 30px;
      margin-top: 30px;
      width: 700px;
      line-height: 1.6;
    }
    h1 {
      font-size: 32px;
      line-height: 1.6;
      text-align: center;
    }
    </style>
      <img src="hero.jpg" style="width:100%" alt="Cropped triangular front of the Pantheon in Rome.">
    <h1>Day 5 - Rome</h1>
    
    <p>
    So today we decided to visit the Pantheon, it was pretty awesome on the inside but those photos didn't turn out so well. I've included a picture from the outside, you can see how crowded it was!
    </p>
    
    <p>
    The Colosseum is also a must-see for any trip to Rome, it's huge! And it's hard to get a photo which really captures how big it is. The line at the colosseum was long, but if you buy tickets online and show the barcode on your phone it's much faster. The museum inside was pretty awesome too, and comes with an audio guide.
    </p>
    
    <p>
      We found a little gladiator helmet at a souvenir store, so we had to buy it for Federbear. It's a bit big and surprisingly heavy, we think it's actually meant to be a paperweight.
    </p>
    <p>
    <img src="colosseum.jpg" alt="Inside the ruin of the Colosseum with bear wearing gladiator helmet." height="150">
    <img src="trevi.jpg" alt="The Trevi Fountain."height="150">
    <img src="pantheon.jpg" alt="Outside view of the Pantheon." height="150">
    <img src="inside.jpg" alt="Inside, looking up at the domed ceiling of the Pantheon." height="150"></p>
    <p>
    As a last bit of fun, I'm not sure where this was from, but this Lion has the weirdest facial expression, and check out the tiny bird perched on top!
    </p>
    <p>
      <img src="lion.jpg" alt="Statue of a lion with a small bird on the head." width="700"></p>
    ```
    

cheatto sheeto