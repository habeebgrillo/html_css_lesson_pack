====================================================================================================================================================
                                                            INTRODUCTION
====================================================================================================================================================

<!-- comment --> // this is used to make a comment in your html file and does not show up in your browser.

<!DOCTYPE html>         <!-- this is the start of every html file --> (Step 1)
<html>                   <!-- and this is the next part --> (Step 2)
<head>                    (Step 3)
    <title> </title>    <!-- title tag-->  (Step 4)
                         <!-- this tag also contains your meta data tags and scripts -->
</head>

<body>            (Step 5)
                            <!-- this is where all your page contents is contained in, like image tags, forms, text, links -->
    <h1></h1>
    <h2></h2>                <!-- These are all different headings and sizes-->
    <h3></h3>
    <h4></h4>
    <h5></h5>
    <h6></h6>
    <p></p>

</body>

</html>

<!-- install live server extension to view your page via http protocol & you wont have to load the page every time -->
<!-- use google chrome inspect/developer tool to view -->
    
Summary
- HTML is markup language to structure content
- CSS is the language used to style web pages
- How to create HTML file using VS Code as our editor
- Seen what HTML tags are and how we use them
- Know that the visible part of a web page goes in the < body> tag
- Seen how to preview the HTML page in a browser



=======================================================================================================================================================
                                                                    HTML TAGS & BASICS
=======================================================================================================================================================

 
<strong> </strong>            <!-- this is used to make a text bold -->

<em> </em>                    <!-- this is used to make a text italics -->

<small> </small>              <!-- this is used to make a text slightly smaller -->

<ul>                          <!-- this is used to make unordered list and its a wrapper for <li> tag, e.g bullet points -->
    <li> </li>                <!-- this contains the actual list -->
</ul>

<ol>                          <!-- this is used to make ordered list and its a wrapper for <li> tag  e.g number list-->
    <li> </li>                <!-- this contains the actual list -->
</ol>    

<div> </div>                  <!-- "division" tag helps to divide contents into sections or group them together -->

<span> </span>                <!-- this is used to add css or js hooks into a part of text and can be used to surround content-->
    
<!--  below are self closing tags and some with attributes-->

<br> or </br>                 <!-- this is used to go to a new line and does not have closing tag -->

<hr> or </br>                 <!-- this is used to make a horizontal row in html and does not close -->

<img src="">                  <!-- this is used to add an image and has to have the "src" attribute that points to a folder/file or image address and the "alt" attribute is used for screen readers, like a description of the image, but its just for accessibility cuz it does not display-->

<a href="">                   <!-- anchor tags are used to link pages or add links to pages "href - hyperlinks reference", this attribute points to the exact link we want to go to and the link in the middle of " " or a file path to one of our pages in our local directory -->

<blockquote cite="">          <!-- used to add another quote from a different/original source into your page and add the link into the " "--> 

</blockquote>  

<p style="">                  <!-- style attribute is used to do inline CSS in your html file and add colors/styling   -->


Summary
- Learnt some of the most common HTML tags in web pages
-p, ul, Li, div, a, img, etc
- Talked about attributes (sc, href, cite, alt etc)
- How to create comments in an HTML file


====================================================================================================================================================
                                                    HTML WEB FORM TAGS
====================================================================================================================================================

<form action="">                         <!-- This contains all your input fields --> <!-- actions are used in server-side-->


<input type="text">            <!-- This specifies the type of input, text or numbers or emails-->

<input type="text" id="username">      <!-- "id" is an identifier and it is unique, no other tag should have the "id" name that has been used already, and other tags/element above can also have an "id", they can also be used in css or js, or to link to a label tag-->

===
for text-fields
===============

<label for="username">Enter username:</label>         <!-- the "label" is asking what input field it is "for", the "for" then points to "id" that has been named in the input tag. it will then link it with the input of text and display the "Enter username:" just before the "Text Box" that accepts "text" -->



<label for="email">Enter Email:</label>              <!-- and then this process can be repeated for email and the browser will interpret the textbox/textfield as an email field  -->
<input type="email" id="email">

<label for="password">Enter password:</label>        <!-- repeat the same for password as well -->
<input type="password" id="password">
       
<input type="text" id="username" name="">            <!-- it is a good practice used to grouping input fields together to add the "name" field, it is important for back end developers and used for server side processing and it is standard practice to also give them the same name as the "type" and "id"--> 

===
for radio buttons
=================

 <form action="">                                      <!-- it also helps to group form fields together and restricts the browser from multiple selections on radio buttons if they had different "name" fields  -->
‹input type="radio" name="gender" value="male" > Male<br> <!-- When a user clicks on a radio-button, it becomes checked, & all other radio-buttons with equal name become unchecked -->

‹input type="radio" name="gender" value="female" > Female<br>

‹input type="radio" name="gender" value="other"> Other  <!-- the "value" field is given by the developer directly, rather than taking it from the user using the "label", the "value" field can be used directly in an input tag since there is no need for a textfield from the user, using "label" tag. and the server can read the value and see what has been selected-->


<input type="radio" name="age" value="26-50" id="option-2">        <!-- the "value" field is good to add as a standard, for server-side developer -->
<label for="option-2">26-50</label>        <!-- remember that label is just so that the user can see the "option-2"  which the "value" has already been determined and the "label" uses the "for" to point to the "id"   -->


====
for dropdowns in a form
=======================                   

<label for="question">Security question:</label>            
<select name="question" id="question">                             <!-- the select tag is used for drop downs and you can nest different things in it -->
    <option value="q1">What is your favourite pet name?</option>    <!-- the option tag is in the select tag and the option tag has a "value" field just as we learnt above. However, depending on what was selected as option, the value goes to the server-->  <!-- and you can have a textfield to accept and type the answers-->
</select>
<label>


===
text area
============

<textarea name="bio" id="bio" cols="30" rows="10" placaholder="about you..."></textarea>    <!-- Text area tag is for large number of texts --> <!-- cols and rows is how wide or how long you want it to be displayed, it can also be changed using css --> <!-- placeholder attribute is used as text suggestion in the textarea box, and it is displayed to the user and disappears when user starts to type and it can be added to input tags as well-->


===
submit buttons
===============

<input type="submit" value="submit form">            <!-- the "submit" send the values entered in all the form fields by the user, it sends it to the backend or to the "form action". and the "value" is what the user sees in the submit button-->

===
required                             <!-- the "required" attribute ensures that a certain input field must accept a value before the form can be submitted, and it is always set to true by default-->
=================



</form>                 

Summary
- How to create a web form and what the 'action' attribute is for
- Seen a lot of the most common input types
- text, email, password, radio, select, textarea
- How to use labels, the id attribute & the name attribute
- How forms are submitted and validated



====================================================================================================================================================
                                                                    CSS BASICS
====================================================================================================================================================

===
CSS RULES
=========
- CSS can be written inline(inside a tag) or can be written externally (in an external folder)
- CSS can also be written standalone in the style tag in the head section of html
- every declaration for a selector must begin with an opening curly brace and end with a closing curly brace.
- a code block would have a property/key name and must start with a colon ":" and value that ends with a semicolon ";"
- external css is better when targeting a property or tag in different/multiple pages and you want them to have the same value.
- 

                                        <!-- selectors are what we want to actually target on a webpage and there are different types of selectors-->

this is called selectors------->    div{ <!-- whatever is between the curly braces code blocks is called "declarations" it has a "key" and "value" pair or "property" and "value" pairs -->
                                        color: red;
                                        margin: 20px;            
                                       }                

this is called selectors------->    li{
                                        font-weight: bold;
                                    }