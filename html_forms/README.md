HTML-Forms

syntax:
<form action="/my-handling-form-page" method="post">…</form>

it is standard practice to set the action and method attribute
Action attribute defines the location(url) ie where the form's collected data should be sent when submitted

method attribute defines which http method to send the data with

*the <label>, <input> and <textarea> elements*
<form action='oururl' method='post'>
<label for='name'>Name</label>
<input type='text> id='name' name='user_name' placeholder='yourname'>
<label for='msg'>Message:</label>
<textarea id='msg' name='user_mssg'><textarea>
</form>

*<button> element
<li class="button">
  <button type="submit">Send your message</button>
</li>
The <button> element also accepts a type attribute — this accepts one of three values: submit, reset, or button.

-A click on a submit button (the default value) sends the form's data to the web page defined by the action attribute of the <form> element.
-A click on a reset button resets all the form widgets to their default value immediately. From a UX point of view, this is considered bad practice, so you should avoid using this type of button unless you really have a good reason to include one.
-A click on a button button does nothing! That sounds silly, but it's amazingly useful for building custom buttons — you can define their chosen functionality with JavaScript.


*Basic form styling*

First of all, add a <style> element to your page, inside your HTML head
<head>
    <style>
        add the css styles
    </style>
</head>


*sending form data to the web*
 We provide a name attribute for each formcontrol.The names are important on both the client- and server-side; they tell the browser which name to give each piece of data and, on the server side, they let the server handle each piece of data by name. The form data is sent to the server as name/value pairs.

 To name the data in a form, you need to use the name attribute on each form widget that will collect a specific piece of data. Let's look at some of our form code again:

html

<form action="/my-handling-form-page" method="post">
  <ul>
    <li>
      <label for="name">Name:</label>
      <input type="text" id="name" name="user_name" />
    </li>
    <li>
      <label for="mail">Email:</label>
      <input type="email" id="mail" name="user_email" />
    </li>
    <li>
      <label for="msg">Message:</label>
      <textarea id="msg" name="user_message"></textarea>
    </li>

    …
  </ul>
</form>
In our example, the form will send 3 pieces of data named "user_name", "user_email", and "user_message". That data will be sent to the URL "/my-handling-form-page" using the HTTP POST method.

