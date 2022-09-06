## HTML Tag Summary
- HTML Layout
    --------------------------
            <header>
    --------------------------
            <nav>
    --------------------------
                |
    <section> |
                |
    ------------|  <aside>
                |
    <article> |
                |
    --------------------------
            <footer>
    --------------------------
        <header> - Defines a header for a document or a section
        <nav> - Defines a set of navigation links
        <section> - Defines a section in a document
        <article> - Defines an independent, self-contained content
        <aside> - Defines content aside from the content (like a sidebar)
        <footer> - Defines a footer for a document or a section
        <details> - Defines additional details that the user can open and close on demand
        <summary> - Defines a heading for the <details> element

   
- Insider Head tag
    <meta> tag: Describe metadata within an HTML document
        * example
            <meta charset="UTF-8">
            <meta name="description" content="Free Web tutorials">
            <meta name="keywords" content="HTML, CSS, JavaScript">
            <meta name="author" content="John Doe">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <base> tag: Specify a default URL and a default target for all links on a page
    <link> tag: is most often used to link to external style sheets or to add a favicon to your website.
        e.g. <link rel="stylesheet" href="styles.css">
    <style> tag: element to apply a simple style sheet to an HTML document
       * example
       <style>
         h1 {color:red;}
         p {color:blue;}
       </style>

    <title> tag: name of document of tab in the 
    * example
    <head>
       <base href="https://www.w3schools.com/" target="_blank">
       <title>Title of the document</title>
    </head>

    <body>
       <img src="images/stickman.gif" width="24" height="39" alt="Stickman">
       <a href="tags/tag_base.asp">HTML base Tag</a>
    </body> 
- Inside Footer tag
    <footer> tag: footer for a document or section.
        * element typically contains:
            authorship information
            copyright information
            contact information
            sitemap
            back to top links
            related documents
    - Address tag displays italic text inside <address> ... </address>
        <address>
            Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br>
            Visit us at:<br>
            Example.com<br>
            Box 564, Disneyland<br>
            USA
        </address> 
- Embed a client-side javascript
    <script>
        * example
         <script>
            document.getElementById("demo").innerHTML = "Hello JavaScript!";
         </script> 
- Text decorations (it can be replaced by richer CSS)
    <h1>~<h6>: heading text-size
    <b> : bold text
    <strong>: same as <b>
    <em>: italic text
    <i> : italic text or <i class="fas fa-cloud"></i> for icon from https://fontawesome.com/icons
    <mark> : highlighted text
    <sup> : tag defines superscript text.
    <sub> : tag defines subscript text. 

    <q> tag: defines a short quotation.

    <s> tag: specifies text that is no longer correct, accurate or relevant. The text will be displayed with a line through it.
    <del> : line in the middle of text. The text will be displayed with a line through it.
    <ins> : under line from text

    <cite> : italic text - tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.
    <code> tag is used to define a piece of computer code. The content inside is displayed in the browser's default monospace font. 

- Abbreviation of world (when mouse is over WHO, it shows World Health Organization)
    The <abbr title="World Health Organization">WHO</abbr> was founded in 1948. 

- Link to href
    <a> tag defines a hyperlink. It has the following syntax:
    <a href="url">link text</a>

- Image mapping for link 
    * <map> <area> tag
    <map>tag : make areas in the image as link to go by clicking the defined area
    * example
    <img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
    <map name="workmap">
       <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
       <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
       <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
    </map> 

- Content area according to context purpose
    <div> (block element): The tag defines a division or a section in an HTML document.
    <span> (inline element) tag is an inline container used to mark up a part of a text, or a part of a document and easily styled by CSS or manipulated with JavaScript using the class or id attribute.
    <section> tag defines a section in a document.
    <p> tag: defines a paragraph.
    <pre> element is displayed in a fixed-width font, and the text preserves both spaces and line breaks. The text will be displayed exactly as written in the HTML source code.
    <article> : for forum post, blog post, News story
        - Inside article it can have <header> tag
        <article>
            <header>
                <h1>A heading here</h1>
                <p>Posted by John Doe</p>
                <p>Some additional information here</p>
            </header>
            <p>Lorem Ipsum dolor set amet....</p>
        </article>
    <aside> : for sidebar
    <details> : for specifing additional details that the user can open and close on demand
      * example
      <details>
       <summary>Epcot Center</summary>
       <p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions,        international   pavilions, award-winning fireworks and seasonal special events.</p>
      </details> 
      Note: The <summary> tag is used in conjunction with <details> to specify a visible heading for the details.
      <embed> element can also be used to include HTML in HTML:
        e.g. <embed width="100%" height="500px" src="snippet.html"> 
    
- Multi-media controls tags
    * Audio control
     <audio controls>
       <source src="horse.ogg" type="audio/ogg"> -- choose first one
       <source src="horse.mp3" type="audio/mpeg"> -- if not working with first one then second one is palyed
       Your browser does not support the audio tag. -- lastly everythin is not working this comment shows 
    </audio> 

    * Video cotrol
        <video width="320" height="240" controls>
           <source src="movie.mp4" type="video/mp4">
           <source src="movie.ogg" type="video/ogg">
           Your browser does not support the video tag.
        </video> 
    * play Youtube (Add mute=1 after autoplay=1 to let your video start playing automatically (but muted).)
        <iframe width="420" height="315"
            src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
        </iframe> 
- Drawing graphics
    <canvas>
- Image handling
    <img> tag: loading image to show
     * example
      <figure>
       <img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600"> 
       <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
       <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
      </figure>
    <svg> tag defines a container for SVG graphics.
     * example
      <svg width="100" height="100">
        <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
      </svg> 

- Line breaker
    <br> : break line
    <hr> : horizontal line

- Navigation
    <nav> tag defines a set of navigation links.
    * example
    <nav>
        <a href="/html/">HTML</a> |
        <a href="/css/">CSS</a> |
        <a href="/js/">JavaScript</a> |
        <a href="/python/">Python</a>
    </nav> 
- Form to submit data to server
    The target attribute specifies where to display the response that is received after submitting the form. The target attribute can have one of the following values:
    ------------------------------------------------------------
     target Value 	Description
     ------------------------------------------------------------
    _blank 	The response is displayed in a new window or tab
    _self 	The response is displayed in the current window
    _parent 	The response is displayed in the parent frame
    _top 	The response is displayed in the full body of the window
    framename 	The response is displayed in a named iframe
    ------------------------------------------------------------
    The default value is _self which means that the response will open in the current window.

    The <form> element can contain one or more of the following form elements:
            <input>
            <textarea>
            <button>
            <select>
            <option>
            <optgroup>
            <fieldset>
            <label>
            <output>
    - One Line Input
    <input>
    * input attributes
     - 'value="intit value" ' attribute specifies an initial value for an input field.
     - 'readonly' attribute specifies that an input field is read-only.
     - 'disabled' attribute specifies that an input field should be disabled.
     - 'size="20" ' attribute specifies the visible width, in characters, of an input field.
     - 'maxlength="4" ' attribute specifies the maximum number of characters allowed in an input field.
     - 'min="1" ' and 'max="10" ' attributes specify the minimum and maximum values for an input field.
     - 'multiple' attribute specifies that the user is allowed to enter more than one value in an input field. (works with the following input types: email, and file.)
     - 'pattern' attribute specifies a regular expression that the input field's value is checked against, when the form is submitted (works with the following input types: text, date, search, url, tel, email, and password)
     - 'placeholder' attribute specifies a short hint that describes the expected value of an input field (a sample value or a short description of the expected format).
     - 'step' attribute specifies the legal number intervals for an input field. (input types: number, range, date, datetime-local, month, time and week)
     - 'autofocus' attribute specifies that an input field should automatically get focus when the page loads.
     - 'autocomplete="on" ' attribute specifies whether a form or an input field should have autocomplete on or off
        * example
        <form action="/action_page.php" autocomplete="on">
            <label for="fname">First name:</label>
            <input type="text" id="fname" name="fname"><br><br>
            <label for="lname">Last name:</label>
            <input type="text" id="lname" name="lname"><br><br>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" autocomplete="off"><br><br>
            <input type="submit" value="Submit">
        </form>
     - 'list' attribute refers to a <datalist> element that contains pre-defined options for an <input> element
        * example
         <form>
            <input list="browsers">
            <datalist id="browsers">
                <option value="Internet Explorer">
                <option value="Firefox">
                <option value="Chrome">
                <option value="Opera">
                <option value="Safari">
            </datalist>
        </form> 
      * <input type='...'> : changed the input type by selecting type
        <input type="button">
        <input type="checkbox">
        <input type="color">
        <input type="date">
        <input type="datetime-local">
        <input type="email">
        <input type="file">
        <input type="hidden">
        <input type="image">
        <input type="month">
        <input type="number">
        <input type="password">
        <input type="radio">
        <input type="range">
        <input type="reset">
        <input type="search">
        <input type="submit">
        <input type="tel">
        <input type="text"> (default value)
        <input type="time">
        <input type="url">
        <input type="week">
    - Multi Line input
        <textarea> tag defines a multi-line text input control.
    - Drop down menu
        <select> element is used to create a drop-down list.
        * example:
            <label for="carsid">Choose a car:</label>
            <select name="cars" id="carsid">
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="mercedes">Mercedes</option>
                <option value="audi">Audi</option>
            </select> 
            * example with option group
            <label for="cars">Choose a car:</label>
            <select  name="cars" id="cars">
                <optgroup label="Swedish Cars">
                    <option value="volvo">Volvo</option>
                    <option value="saab">Saab</option>
                </optgroup>
                <optgroup label="German Cars">
                    <option value="mercedes">Mercedes</option>
                    <option value="audi">Audi</option>
                </optgroup>
            </select> 
    - Group box 
        <fieldset> : tag is used to group related elements in a form and draws a box around the related elements
        * example
        <form action="/action_page.php">
            <fieldset>
                <legend>Personalia:</legend>
                <label for="fname">First name:</label>
                <input type="text" id="fname" name="fname"><br><br>
                <label for="lname">Last name:</label>
                <input type="text" id="lname" name="lname"><br><br>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email"><br><br>
                <label for="birthday">Birthday:</label>
                <input type="date" id="birthday" name="birthday"><br><br>
                <input type="submit" value="Submit">
            </fieldset>
        </form> 
    - Button for Action
      <button type=''> type: button, reset, submit (with form tag)

- List out and organize data
    <ul> tag defines an unordered (bulleted) list.
        * example
        <ul>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Milk</li>
        </ul> 
    <ol> tag defines an unordered (number) list.
        * example
        <ol>
            <li>Coffee</li>
            <li>Tea</li>
            <li>Milk</li>
        </ol>
    * Describe terms
     <dl>
      <dt>Coffee</dt>
       <dd>Black hot drink</dd>
      <dt>Milk</dt>
       <dd>White cold drink</dd>
     </dl> 
    * tagle tag
    <table>
      <caption>Monthly savings</caption>
      <colgroup>
       <col span="2" style="background-color:red">
       <col style="background-color:yellow">
      </colgroup>
      <thead>
            <tr>
            <th>Month</th>
            <th>Savings</th>
            </tr>
      </thead>
      <tbody>
            <tr>
            <td>January</td>
            <td>$100</td>
            </tr>
            <tr>
            <td>February</td>
            <td>$80</td>
            </tr>
      </tbody>
      <tfoot>
            <tr>
            <td>Sum</td>
            <td>$180</td>
            </tr>
      </tfoot>
    </table>    
    
    

- Progress indicatiors
    <meter> tag defines a scalar measurement within a known range, or a fractional value. This is also known as a gauge.
      * example: 
        <label for="disk_c">Disk usage C:</label>
        <meter id="disk_c" value="2" min="0" max="10">2 out of 10</meter><br>
    <progress> tag represents the completion progress of a task.
      * example:
        <label for="file">Downloading progress:</label>
        <progress id="file" value="32" max="100"> 32% </progress>   

- ** Here are the block-level elements in HTML:
    <div> <address> <article>  <aside> <blockquote> <canvas>
    <dd> <dl> <dt> <fieldset>  <figcaption> <figure>
    <footer> <form> <h1>-<h6> <header> <hr> <li>
    <main> <nav> <ol> <p> <pre> <section> <table> <tfoot> <ul> <video>
- ** inline container used to mark up a part of a text, or a part of a document:
    <span> 
    <a>
    <i>
    <img>

- Geolocation 
    <body>

    <p>Click the button to get your coordinates.</p>

    <button onclick="getLocation()">Try It</button>

    <p id="demo"></p>

    <script>
        var x = document.getElementById("demo");

        function getLocation() {
        if (navigator.geolocation) {
            navigator.geolocation.getCurrentPosition(showPosition, showError);
        } else { 
            x.innerHTML = "Geolocation is not supported by this browser.";
        }
        }

        function showPosition(position) {
        x.innerHTML = "Latitude: " + position.coords.latitude + 
        "<br>Longitude: " + position.coords.longitude;
        }

        function showError(error) {
        switch(error.code) {
            case error.PERMISSION_DENIED:
            x.innerHTML = "User denied the request for Geolocation."
            break;
            case error.POSITION_UNAVAILABLE:
            x.innerHTML = "Location information is unavailable."
            break;
            case error.TIMEOUT:
            x.innerHTML = "The request to get user location timed out."
            break;
            case error.UNKNOWN_ERROR:
            x.innerHTML = "An unknown error occurred."
            break;
        }
        }
    </script>

    </body>
- HTML Web Storage Objects
    HTML web storage provides two objects for storing data on the client:
    - window.localStorage - stores data with no expiration date
    - window.sessionStorage - stores data for one session (data is lost when the browser tab is closed)
