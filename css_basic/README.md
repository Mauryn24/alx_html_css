#CSS
CSS - Cascading Styling Sheets
CSS - styling language that is used for presentation.
    SYNTAX
    selector{
        property1: value;
        property2: value;
    }
    Selector refers to the elements, class or id
            Element css representation
            element{
                property: value;
            }
            class css representation
            .class-name{
                property: value;
            }
            ID css representation
            #id{
                property: value;
            }
HOW TO LOAD CSS
CSS can be loadded using
1. inline styling method
     Inline styles directly affect the tag they are written in, without the use of selectors.
     For example <p style="color: blue; font-size: 46px;">
2. style element
    defined in the <head> section of an HTML page, within a <style> element.
    For Example
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
3. external method
To use an external style sheet, add a link to it in the <head> section of each HTML page
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
The external style sheet can be written in any text editor. The file must not contain any HTML code, and must be saved with a .css extension.