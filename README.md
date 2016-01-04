http://img.f-i-h.info/66ee6f9ed0f22977b202b413cea133ab.png
# Description
This is the original ShadowBox JS taken from www.shadowbox-js.com


Shadowbox was designed with both the web hobbyist and the experienced programmer in mind. As such, it can easily
be added to any web page with very little time and effort using the default settings. At the same time, Shadowbox offers
a great deal of flexibility for those users who need to fine-tune the details of its appearance and operation for a given
project.
This page contains detailed instructions on how to set up and run Shadowbox from both perspectives.


# Installation
After you download a copy of the code with all of the options you need, decompress the archive (unzip it) and upload
the entire folder to your web server. The exact location is not important since Shadowbox will automatically detect
where it is installed when it runs. However, it is important that you keep all of the files together. After you have uploaded
the code to your server, simply link to the JavaScript and CSS files as described below.

# Setup
The simplest way to set up Shadowbox is to include the JavaScript and CSS files in the <head> of your document (web
page) and then call Shadowbox.init, like this:
<code>
    <link rel="stylesheet" type="text/css" href="shadowbox.css">
    <script type="text/javascript" src="shadowbox.js"></script>
    <script type="text/javascript">
    Shadowbox.init();
    </script>
</code>

The following example is a bit more complex and uses an object literal to specify some options. Options passed to this
method will become the default for all instances of Shadowbox on the page.
<code>
    <link rel="stylesheet" type="text/css" href="shadowbox.css">
    <script type="text/javascript" src="shadowbox.js"></script>
    <script type="text/javascript">
    Shadowbox.init({
     handleOversize: "drag",
     modal: true
    });
    </script>
</code>

# Markup
Next you need to tell Shadowbox which links you want it to open. The simplest way to do this is through your HTML
markup. If you're going to take this route, at the very least you must add a rel="shadowbox" attribute to each link. For
example, say you have this link to an image on your page:
<code><a href="myimage.jpg">My Image</a></code>

In order to set up this link for use with Shadowbox, simply change it to this:
<code><a href="myimage.jpg" rel="shadowbox">My Image</a></code>


That's it! Clicking on this link should now open up the image in Shadowbox

For more docs go here - http://udel.edu/~aadavis/educ286/shadowbox/Shadowbox.js%20%BB%20Usage.pdf