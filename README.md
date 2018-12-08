# Snackbar
## Introduction:
Snackbar is considered as a UI(User Interface) element which we usually used for feedback of the user, especially when an instantaneous feedback is required from the user after the action is performed. Snackbar appears at the bottom of screen and if Coordinator Layout is used as its parent, it can be dispersed by swiping.

## History:
Snackbar was introduced in Android Systems in **API# 22.2.0**. The package library needed to import in activity to implement features of snackbar is **android.support.design.widget.BaseTransientBottomBar<android.support.design.widget.Snackbar>**.

## Major Methods:
### 1.make
This method is used to make a snackbar to display a message.<br>
Below is the declaration of make function which consists of parameters and return type.<br>
**Snackbar make (View view,CharSequence text,int duration)**<br>
**Parameters:**<br>
view	View: The view to find a parent from.<br>
text	CharSequence: The text to show. Can be formatted text.<br>
duration	int: How long to display the message. Either LENGTH_SHORT or LENGTH_LONG<br>
**Ruturns:**<br>
Snackbar<br>

There is another way in which we can provide a resource id of the string instead of providing a proper text. For that we have to change the second parameter of the above function.
Instead of using text CharSequence we can use a simple int type to get access to id of the string resourse. Below I am providing the syntax for another form:<br><br>
**Snackbar make (View view, int resId, int duration)**, Where second parameter can be described as below:<br>
resId	int: The resource id of the string resource to use. Can be formatted text.

### 2.setAction
Set the action to be displayed in this BaseTransientBottomBar.<br>
**Snackbar setAction (CharSequence text, View.OnClickListener listener)**<br>
**Parameters:**<br>
text	CharSequence: Text to display for the action<br>
listener	View.OnClickListener: callback to be invoked when the action is clicked<br>
**Returns:**<br>
Snackbar<br>

### 3.setActionTextColor
**Snackbar setActionTextColor (ColorStateList colors)**<br>
Sets the text color of the action specified in setAction(CharSequence, View.OnClickListener).<br>
**Parameters:**<br>
colors	ColorStateList<br>
**Returns:**<br>
Snackbar<br>

### 4.setActionTextColor
**Snackbar setActionTextColor (int color)**<br>
Sets the text color of the action specified in setAction(CharSequence, View.OnClickListener).<br>
**Parameters:**<br>
color	int<br>
**Returns:**<br>
Snackbar<br>

### 5.setText
**Snackbar setText (CharSequence message)**<br>
Update the text in this Snackbar.<br>
**Parameters:**<br>
message	CharSequence: The new text for this BaseTransientBottomBar.<br>
**Ruturns:**<br>
Snackbar<br>

### 6.setText
**Snackbar setText (int resId)**<br>
Update the text in this Snackbar.<br>
**Parameters:**<br>
resId	int: The new text for this BaseTransientBottomBar.<br>
**Returns:**<br>
Snackbar<br>









       


