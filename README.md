# FFFM
Flat File file manager


This is a simple flat-file image upload/management script.  I use this one of the Raspberry pi's at church in order to allow people to upload slides to be displayed on the tv.  This is taken from jcampbell1.  I've made a couple slight modifications to better fit our purpose.  By default, this script will display a list of all files in a given directory, however I only wanted it to display jpg files in the given directory and excluded everything else.

I did this by using the following code:

<code>
$list = preg_grep("/^.*\.(jpg)$/i", $list);
</code>

Where $list is an array holding the list of file/folder names in the current directory.
