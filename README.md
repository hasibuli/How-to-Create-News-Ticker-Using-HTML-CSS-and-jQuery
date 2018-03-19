# jQuery News Ticker
Hey, this is S M Hasibu Islam, working web development field from 2009 to till now. If you don’t know how to create a jQuery news ticker, in bellows tutorial I’ll teach you how to create a news ticker using HTML, CSS & jQuery. I just create a news ticker for any website. You can use the ticker to give smooth updates to our viewer in just few clicks.

So, let’s get started core code development stage.

Step: 1

Starts from bellows codes. We have written basic code and include necessary files for getting view of news ticker. It’s just sample code.

<!DOCTYPE html>
<html>
<head>
<title>My jQuery News Ticker</title>
<script type="text/javascript" src=" http://code.jquery.com/jquery-2.2.3.js "></script>
</head>
<body>
</body>
</html>

Step: 2

The second step is to add the HTML code. I have adding some sample HTML code for run this news ticker and use all dummy data as text. To get started creating this, you’ll need to put bellows HTML code into the body tag the.

<div class=“csehasibticker”>
<h3>Breaking News</h3>
<ul id=“csehasibticker”>
<li>Lorem Ipsum is simply dummy text of the printing and typesetting industry...</li>
<li>Lorem Ipsum has been the industry’s standard dummy text ever since the 1500s</li>
<ul>
<li>Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC...</li>
</ul>
<ul>
<li>There are many variations of passages of Lorem Ipsum available...</li>
</ul>
<ul>
<li>All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary...</li>
</ul>
</div>

Step: 3

Our HTML code is included into our main HTML code. Now we need to add jQuery code to run news ticker slide of start action. Now we’ll add bellows jQuey code inside the head tag.

<!-- Include jQery function -->
<script type="text/javascript">
function csehasibticker() {
jQuery('#csehasibticker li:first').slideUp(function() {
jQuery(this).appendTo($('#csehasibticker')).slideDown();
});
}
setInterval(csehasibticker, 4000);
</script>
<!-- //Include jQery function -->

In the above jQuery script, here we write a jQuery function named csehasibticker(). Inside this jQuery function we have slide. Then we call the javascript setInterval() function which run our csehasibticker() function interval of 4 sec.

Step: 4

All are done without style option or view style of the news ticker. Finally we add our CSS inside the head tag or just above the body tag. Any developer can modify the new ticker very easily by modifying bellows CSS code.

<style>
#wrapper{
width:80%;
margin:0 auto;
}
.csehasibticker{
width: 550px;
height: 255px;
overflow: hidden;
border: 1px solid #eee;
border-radius: 5px;
box-shadow: 0px 0px 5px #eee;
background: #00a1e0;
color:#fff;
text-align: left;
margin:0 auto;
}
.csehasibticker h3 {
padding: 0 0 7px 7px;
border-bottom: 1px solid #444;
}
ul {
list-style: none;
padding: 0;
margin: 0;
font-style: italic;
}
ul li {
list-style: none;
height:50px;
padding:7px;
border-bottom: 1px solid #444;
}
</style>

Finally, we have created the news ticker & tested online. I have test this news ticker and its work smoothly.

NB: Next post will depend on viewers comment and questions.
