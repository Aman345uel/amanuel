# Web html

## Class 1 html

My html tags

```html
<h1> web tech</h1>
1. <abbr> Defines an abbreviation or an acronym
2<aside> Defines content aside from the page content
3.<base> Specifies the base URL/target for all relative URLs in a document
4.<template>Defines a container for content that should be hidden when the page loads
5.<figure> Specifies self-contained content
6.<data>	Adds a machine-readable
 translation of a given conten
```

1. List in input

  List: Refers to a <datalist> element that contains pre-defined options for an <input> element

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```

1. <select> Specifies that a user can enter more than one value

```html
<label for="cars">Choose a car:</label>

<select name="cars" id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="mercedes">Mercedes</option>
  <option value="audi">Audi</option>
</select>
```

1. <caption> Defines a table caption

```html
<table>
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```

| 10.https://www.w3schools.com/tags/tag_map.asp | Defines an image map |
| --- | --- |

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
</map>

```

| 11.https://www.w3schools.com/tags/tag_th.asp | Defines a header cell in a table |
| --- | --- |

| 12.https://www.w3schools.com/tags/tag_tr.asp | Defines a row in a table |
| --- | --- |

```html
<table>
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
</table>
```

### 13.

| https://www.w3schools.com/tags/tag_i.asp | Defines a part of text in an alternate voice or mood |
| --- | --- |

### 14.

| https://www.w3schools.com/tags/tag_hgroup.asp | Defines a header and related content |
| --- | --- |

### 15.

| https://www.w3schools.com/tags/tag_noscript.asp | Defines an alternate content for users that do not support client-side scripts |
| --- | --- |

# Tags requested by the teacher

1. Iframe

| https://www.w3schools.com/tags/tag_iframe.asp | Defines an inline frame |
| --- | --- |

```html
<iframe src="https://www.w3schools.com" title="W3Schools Free Online Web Tutorials"></iframe>
```

# 2. The <form> Element

The HTML `<form>` element is used to create an HTML form for user input:

```html
<form>
.
form elements
.
</form>
```

# The <input> Element

The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the `type` attribute.

Here are some examples:

| Type | Description |
| --- | --- |
| <input type="text"> | Displays a single-line text input field |
| <input type="radio"> | Displays a radio button (for selecting one of many choices) |
| <input type="checkbox"> | Displays a checkbox (for selecting zero or more of many choices) |
| <input type="submit"> | Displays a submit button (for submitting the form) |
| <input type="button"> | Displays a clickable button |

# Text Fields

The `<input type="text">` defines a single-line input field for text input.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

# The <label> Element

Notice the use of the `<label>` element in the example above.

The `<label>` tag defines a label for many form elements.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focuses on the input element.

The `<label>` element also helps users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the `<label>` element, it toggles the radio button/checkbox.

The `for` attribute of the `<label>` tag should be equal to the `id` attribute of the `<input>` element to bind them together.

---

# Radio Buttons

The `<input type="radio">` defines a radio button.

Radio buttons let a user select ONE of a limited number of choices.

```html
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

# Checkboxes

The `<input type="checkbox">` defines a **checkbox**.

Checkboxes let a user select ZERO or MORE options of a limited number of choices.

```html
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
```

# The Submit Button

The `<input type="submit">` defines a button for submitting the form data to a form-handler.

The form-handler is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's `action` attribute.

```html
<label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

# The Name Attribute for <input>

Notice that each input field must have a `name` attribute to be submitted.

If the `name` attribute is omitted, the value of the input field will not be sent at all.

```html
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>
```

# 3. Div

# The <div> Element

The `<div>` element is by default a block element, meaning that it takes all available width, and comes with line breaks before and after.

# Example

A <div> element takes up all available width:

```html
Lorem Ipsum <div>I am a div</div> dolor sit amet.
```

# <div> as a container

The `<div>` element is often used to group sections of a web page together.

# Example

A <div> element with HTML elements:

```html
<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>
```

# Aligning <div> elements side by side

When building web pages, you often want to have two or more `<div>` elements side by side, like this:

# London

London is the capital city of England.

London has over 13 million inhabitants.

# Oslo

Oslo is the capital city of Norway.

Oslo has over 600.000 inhabitants.

# Rome

Rome is the capital city of Italy.

Rome has almost 3 million inhabitants.

There are different methods for aligning elements side by side, all include some CSS styling. We will look at the most common methods:

---

# Float

The CSS `float` property was not originally meant to align `<div>` elements side-by-side, but has been used for this purpose for many years.

The CSS `float` property is used for positioning and formatting content and allow elements float next to each other instead of on top of each other.

# Example

How to use float to align div elements side by side:

```html
<style>
.mycontainer {
  width:100%;
  overflow:auto;
}
.mycontainer div {
  width:33%;
  float:left;
}
</style>
```

# Grid

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

Sounds almost the same as flex, but has the ability to define more than one row and position each row individually.

The CSS grid method requires that you surround the `<div>` elements with another `<div>` element and give the status as a grid container, and you must specify the width of each column.

# Example

How to use grid to align <div> elements side by side:

```html
<style>.grid-container 
{  
display: grid;  grid-template-columns: 33% 33% 33%;
}
</style>
```