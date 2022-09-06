- All CSS Simple Selectors

    --------------------------------------------------
    Selector 	Example 	Example description
    --------------------------------------------------
    1. #id 	#firstname 	Selects the element with id="firstname"
    2. .class 	.intro 	Selects all elements with class="intro"
    3. element.class 	p.intro 	Selects only <p> elements with class="intro"
    4. * 	* 	Selects all elements
    5. element 	p 	Selects all <p> elements
    6. element,element,.. 	div, p 	Selects all <div> elements and all <p> elements

- Color control in th any tag
    - background-color: sky (apply it on block background) it can be color name , #ff00ee (hex) and rgba(255,255,255)
    - color: gray (apply it on text )

- Shorten form convention for [margin], [border-style], [padding]
    [margin] or [border-style]: [top] [right] [bottom] [left] (4 values)
    [margin] or [border-style]: [top] [right-left] [bottom]   (3 values)
    [margin] or [border-style]: [top-bottom] [right-left]     (2 values)
    * e.g. : 
        margin: 25px 50px 75px 100px; (4 values)
        margin: 25px 50px  100px;     (3 values)
        margin: 25px 50px ;           (2 values)
        margin: 25px;                 (1 value for all side)



- Background control

    - background-color
    - background-image
    - background-repeat
    - background-attachment
    - background-position
    - background (shorthand property)
    1. background-color
        div {
            background-color: green;
            opacity: 0.3;
        }
      or 
        div {
            background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
        }
    2. background-image
        body {
        background-image: url("img_tree.png");
        background-repeat: no-repeat;,  
                    repeat; (x-ydirection), 
                    repeat-x(horizontally), 
                    repeat-y(vertically)
        background-position: right top;
        background-attachment: scroll; (image move by scroll action)
                             : fixed; (image fixed in view so it stays at same position)
        }
    3. Shorten form
        body {
            background: #ffffff url("img_tree.png") no-repeat right top;
        }


- CSS Box Model - design and layout
    - Margin - Clears an area outside the border. The margin is transparent
    - Border - A border that goes around the padding and content
    - Padding - Clears an area around the content. The padding is transparent
    - Content - The content of the box, where text and images appear
    * e.g.:
    div {
        width: 300px;
        margin: 20px;
        border: 15px solid green;
        padding: 50px;
    }


- Border control
    structure - [border-side]: [width] [style] [color]
    1. [border-side]
        border:        - all side (top, right, bottom, left)
        border-top:
        border-bottom: 
        border-left:
        border-right:
    2. [width] - in px, pt, cm, em, etc
    3. [style] - border style
        dotted - Defines a dotted border
        dashed - Defines a dashed border
        solid - Defines a solid border
        double - Defines a double border
        groove - Defines a 3D grooved border. The effect depends on the border-color value
        ridge - Defines a 3D ridged border. The effect depends on the border-color value
        inset - Defines a 3D inset border. The effect depends on the border-color value
        outset - Defines a 3D outset border. The effect depends on the border-color value
        none - Defines no border
        hidden - Defines a hidden border
    4. [color] - border color
        #00ffee or rgba(r,g,b,alpha-opacity)
    * example
        p {
            border: 2px solid red;
            border-radius: 5px;
        }

- Margin control - Margins are used to create space around elements, outside of any defined borders.
    - margin property
        margin-top:
        margin-right:
        margin-bottom:
        margin-left:
    - shorthen form
        div {
            border: 1px solid black;
            margin: 25px 50px; /* top-bottom right-left */
            background-color: lightblue;
        }
    - margin various values:
        [auto] - the browser calculates the margin
        length - specifies a margin in [px], [pt], [cm], etc.
        [%] - specifies a margin in % of the width of the containing element
        [inherit] - specifies that the margin should be inherited from the parent element


- Margin Collapse Problem

    Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

    This does not happen on left and right margins! Only top and bottom margins!
    * e.g.:
        h1 {
            margin: 0 0 50px 0;
        }

        h2 {
            margin: 20px 0 0 0;
        }
        In the example above, the <h1> element has a bottom margin of 50px and the <h2> element has a top margin set to 20px.

        Common sense would seem to suggest that the vertical margin between the <h1> and the <h2> would be a total of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px (which is selected with largest value).

- Padding Control: Padding is used to create space inside an element's content, inside of any defined borders.
    - Padding - Individual Sides
       CSS has properties for specifying the padding for each side of an element:
        padding-top:
        padding-right:
        padding-bottom:
        padding-left:
    - Shorten form
        padding: t r b l (4 values)
        padding: t r-l b (3 values)
        padding: t-b r-l (2 values)
        padding: t-r-b-1 (1 value)
    * e.g.:
        div {
            border: 1px solid black;
            padding: 25px 50px 75px;
            background-color: lightblue;
        }


- Height and Width of elements 

    [height] : value
    [width] : value
    The [height] and [width] properties are used to set the height and width of an element.
    The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the [padding], [border], and [margin] of the element.

    - The height and width properties may have the following values:
        [auto] - This is default. The browser calculates the height and width
        length - Defines the height/width in [px], [cm], etc.
        [%] - Defines the height/width in percent of the containing block
        [initial] - Sets the height/width to its default value
        [inherit] - The height/width will be inherited from its parent value

    * e.g.:
        div {
            height: 200px;
            width: 50%;
            background-color: powderblue;
        }
    [max-width] - The max-width property is used to set the maximum width of an element.
    [max-height] - The max-height property is used to set the maximum height of an element.
    * e.g.:
        div {
            max-width: 500px;
            height: 100px;
            background-color: powderblue;
        }

-  Text controls
    - Text Color: The color property is used to set the color of the text
        * e.g.:
            h1 {
                background-color: black;
                color: white;
            }
    - Text Alignments:
        - text-align
        - text-align-last
        - direction
        - unicode-bidi
        - vertical-align
        1. text-align: left A text can be left or right aligned, centered, or justified.
            - value = [left] or [right] or [center] or [justify]
            * e.g.:
                div {
                    text-align: justify;
                }
        2. text-align-last: The text-align-last property specifies how to align the last line of a text.
        3. vertical-align: The vertical-align property sets the vertical alignment of an element.
            - value: [baseline] | [text-top] | [text-bottom] | [sub] | [super]
    - Text decorations
        - text-decoration-line
        - text-decoration-color
        - text-decoration-style
        - text-decoration-thickness
        - text-decoration
        1. text-decoration-line: value;
            - value = [overline] | [underline] | [line-through] | combinations
        2. text-decoration-color: #112233 or rgba(r,g,b,a) or name of color for setting the color of line
        * e.g.:
            h2 {
                text-decoration-line: line-through;
                text-decoration-color: blue;
            }
        3. text-decoration-style: property is used to set the style of the decoration line.
            - value = [solid] | [double] | [dotted] | [dashed] | [wavy]
            * e.g.:
                p.ex2 {
                    text-decoration-line: underline;
                    text-decoration-style: wavy; 
                    text-decoration-color: red; 
                }
        4. text-decoration-thickness: property is used to set the thickness of the decoration line.
            - value: [auto] default value. | [%] | [px]
        - Shorten form
            p {
                text-decoration: underline red wavy 1px;
            }
        - remove the under line in <a> tag
            All links in HTML are underlined by default. Sometimes you see that links are styled with no underline. The [text-decoration]: [none]; is used to remove the underline from links, like this:
            a {
                text-decoration: none;
            }
    - text transform - property is used to specify uppercase and lowercase letters in a text.
        [text-transform] : value
        - value =  [uppercase] | [lowercase] | [capitalize]
    - text spacing
        - [[text-indent]]
        - [letter-spacing]
        - [word-spacing]
        - [white-space]
        - [line-height]
        1. [text-indent]: property is used to specify the indentation of the first line of a text:
            * e.g.:
                p {
                    text-indent: 50px;
                }
        2. [letter-spacing]: property is used to specify the space between the characters in a text.
            * e.g:
                h1 {
                    letter-spacing: 5px;
                }

                h2 {
                    letter-spacing: -2px;
                }
        3. [word-spacing] property is used to specify the space between the words in a text.
        4. [white-space] property specifies how white-space inside an element is handled.
            * e.g.: This example demonstrates how to disable text wrapping inside an element
                p {
                    white-space: nowrap;
                }
        5. [line-height] property is used to specify the space between lines:
            * e.g.:
                p.small {
                    line-height: 0.8;
                }

                p.big {
                    line-height: 1.8;
                }
    - text shadow: adds shadow to text
        [text-shadow] : [rightside] [bottomside] [blur] [color]
        - e.g.: 
            // Text-shadow with red neon glow:
            h1 {
                color: white;
                text-shadow: 2px 2px 4px #000000;
            }
            // Text-shadow with red and blue neon glow:
            h1 {
                text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
            }
- 

- 

- 

- 