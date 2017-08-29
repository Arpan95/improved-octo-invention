# improved-octo-invention
<div id="calendar"></div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
<script src="js/jquery-ui-datepicker.min.js"></script>
<script>
    $('#calendar').datepicker({
        inline: true,
        firstDay: 1,
        showOtherMonths: true,
        dayNamesMin: ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat']
    });
</script>
.ui-datepicker,
.ui-datepicker table,
.ui-datepicker tr,
.ui-datepicker td,
.ui-datepicker th {
    margin: 0;
    padding: 0;
    border: none;
    border-spacing: 0;
}
.ui-datepicker {
    display: none;
    width: 294px;
    padding: 35px;
    cursor: default;
 
    text-transform: uppercase;
    font-family: Tahoma;
    font-size: 12px;
 
    background: #141517;
 
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    border-radius: 3px;
 
    -webkit-box-shadow: 0px 1px 1px rgba(255,255,255, .1), inset 0px 1px 1px rgb(0,0,0);
    -moz-box-shadow: 0px 1px 1px rgba(255,255,255, .1), inset 0px 1px 1px rgb(0,0,0);
    box-shadow: 0px 1px 1px rgba(255,255,255, .1), inset 0px 1px 1px rgb(0,0,0);
}
.ui-datepicker-header {
    position: relative;
    padding-bottom: 10px;
    border-bottom: 1px solid #d6d6d6;
}
 
.ui-datepicker-title { text-align: center; }
 
.ui-datepicker-month {
    position: relative;
    padding-right: 15px;
    color: #565656;
}
 
.ui-datepicker-year {
    padding-left: 8px;
    color: #a8a8a8;
}
.ui-datepicker-month:before {
    display: block;
    position: absolute;
    top: 5px;
    right: 0;
    width: 5px;
    height: 5px;
    content: '';
 
    background: #a5cd4e;
    background: -moz-linear-gradient(top, #a5cd4e 0%, #6b8f1a 100%);
    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,#a5cd4e), color-stop(100%,#6b8f1a));
    background: -webkit-linear-gradient(top, #a5cd4e 0%,#6b8f1a 100%);
    background: -o-linear-gradient(top, #a5cd4e 0%,#6b8f1a 100%);
    background: -ms-linear-gradient(top, #a5cd4e 0%,#6b8f1a 100%);
    background: linear-gradient(top, #a5cd4e 0%,#6b8f1a 100%);
 
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
}
.ui-datepicker-prev,
.ui-datepicker-next {
    position: absolute;
    top: -2px;
    padding: 5px;
    cursor: pointer;
}
 
.ui-datepicker-prev {
    left: 0;
    padding-left: 0;
}
 
.ui-datepicker-next {
    right: 0;
    padding-right: 0;
}
 
.ui-datepicker-prev span,
.ui-datepicker-next span{
    display: block;
    width: 5px;
    height: 10px;
    text-indent: -9999px;
 
    background-image: url(../img/arrows.png);
}
 
.ui-datepicker-prev span { background-position: 0px 0px; }
 
.ui-datepicker-next span { background-position: -5px 0px; }
 
.ui-datepicker-prev-hover span { background-position: 0px -10px; }
 
.ui-datepicker-next-hover span { background-position: -5px -10px; }
Step 5 – Calendar Styles

To style the days of the week we will add a top and bottom padding and change the color.
1
2
3
4
5
6
7
8
	
.ui-datepicker-calendar th {
    padding-top: 15px;
    padding-bottom: 10px;
 
    text-align: center;
    font-weight: normal;
    color: #a8a8a8;
}

Then we will style the “days grid” by adding some paddings, changing the colors and we will add a transparent border to each number. This is needed because we will add a border to the active number so to avoid it to jump when we click on a number we need to add this transparent border.
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
	
.ui-datepicker-calendar td {
    padding: 0 7px;
 
    text-align: center;
    line-height: 26px;
}
 
.ui-datepicker-calendar .ui-state-default {
    display: block;
    width: 26px;
    outline: none;
 
    text-decoration: none;
    color: #a8a8a8;
 
    border: 1px solid transparent;
}

For the active state we will change the text and border color to green. For the “other months days” we will change the color to a darker one.
1
2
3
4
5
6
	
.ui-datepicker-calendar .ui-state-active {
    color: #6a9113;
    border: 1px solid #6a9113;
}
 
.ui-datepicker-other-month .ui-state-default { color: #565656; }
Conclusion

We finished our calendar. If you have any question let me know in the comments. Also don’t forget to leave some feedback and share it with your friends. Follow us if you want to be the first to know about the latest tutorials and articles.

Preview
Download Calendar
Sign in to Download

Just click one of the buttons below to get instant access.

Your account is 100% secured and safe from spam!
error
Sign in via Twitter
Sign in via Google
By clicking on the button(s), you agree with Terms of Use, Privacy Policy

Related Posts

    Best Free JS Libraries for Custom Radios & Checkboxes Best Free JS Libraries for Custom Radios & Checkboxes
    Create a Product Page with Interactive Colors in HTML, CSS3 & jQuery Create a Product Page with Interactive Colors in HTML, CSS3 & jQuery
    Create a Full-Screen Slider Using HTML, CSS3 and jQuery Create a Full-Screen Slider Using HTML, CSS3 and jQuery

Newsletter

Get our products/news earlier than others, let’s get in touch.
12 Comments

    Piero Recchia Apr 4, 7:28 pm

    Great tutorial thanks a lot, is posible add click event on a day to show something or go to url?
    Reply
        Valeriu Apr 4, 7:34 pm

        Thanks Piero! As this calendar is based on jQuery UI Datepicker I think you can add this click events. Just try to google “jquery datepicker events” I’m sure you will find some help.
        Reply
    Luch Jun 27, 6:38 pm

    thanks for the tutorial, btw, u forgot to link us the js, and the arrow images (wich i spend a lot of times cursing and asking why they f*** wouldn’t show), i found that in the css there was this line >> background-image: url(../img/arrows.png);

    thanks anyways! :), it looks really good
    Reply
    Alok Nath Agarwal Oct 9, 2:18 pm

    Good Day !!

    My friend shared it with me. I want to add this onto my site – kushalastrology.com. I was searching since long. This may fulfil my requirement. am a quite fresher in .php. hope so, it will work. Also need a hover date picker.

    Even Thanks a lot..
    Reply
    dinesh kumar Apr 18, 2:22 pm

    tanks for this tutorial but i have a problem how can i implement with wordpress and CI
    Reply
    TwoStarII Jul 13, 11:31 pm

    Firstly Thanks For The Code.

    How do we add events to the calendar?
    How do we make an event pop up box when mouse hovers over marked event?
    Reply
    Amin Jul 23, 1:08 am

    Hi) It’s so very cool calendar) but i don’t know that how i can get selected day in calendar!!! can you help me, please???
    Reply
    Mike Oct 8, 3:38 pm

    The src file is jquery.ui.datepicker.min.js not
    jquery-ui-datepicker.min.js
    Reply
    Maxine Aug 11, 9:59 am

    Hi, Great styling! Clean and Simple!.

    Do you know if jquery can change the background of each date? example if

    August 10 background is green
    August 11 background is yellow

    something like that.

    Thank you!
    Reply
    Mirte Nov 5, 12:05 pm

    thanks for this tutorial. It worked perfectly for me in combination with datepicker and impromptu just a couple of days ago, but now it doesnt show up anymore and i dont have a clue why.. maybe there’s anyone out here who can have a short look?

    MY HTML document looks similar to this:
    ….

    …..
    ….

    ….
    ….

    …..
    …..

    $(‘.ui-datepicker’).datepicker({
    inline: true,
    firstDay: 1,
    showOtherMonths: true,
    dayNamesMin: [‘Zo’, ‘Ma’, ‘Di’, ‘Wo’, ‘Do’, ‘Vr’, ‘Za’]
    });

    var events = [
    { Title: “Signeersessie Boekenbeurs 14:00u – 16:00u Antwerpen Expo Zaal 2 – Standnummer 202 Jan van Rijswijcklaan 191, 2020 Antwerpen”, Date: new Date(“10/31/2015”)},
    { Title: “Signeersessie Boekenbeurs 14:00u – 16:00u Antwerpen Expo Zaal 2 – Standnummer 202 Jan van Rijswijcklaan 191, 2020 Antwerpen”, Date: new Date(“11/1/2015”) }
    ];

    $(“#calendar”).datepicker({
    beforeShowDay: function(date) {
    var result = [true, ”, null];
    var matching = $.grep(events, function(event) {
    return event.Date.valueOf() === date.valueOf();
    });

    if (matching.length) {
    result = [true, ‘highlight’, null];
    }
    return result;
    },
    onSelect: function(dateText) {
    var date,
    selectedDate = new Date(dateText),
    i = 0,
    event = null;

    while (i < events.length && !event) {
    date = events[i].Date;

    if (selectedDate.valueOf() === date.valueOf()) {
    event = events[i];
    }
    i++;
    }
    if (event) {
    $.prompt(event.Title);
    }
    }
    });

    Thanks in Advance!
    Reply
        Mirte Nov 5, 12:08 pm

        Looks like the first part is missing..

        There i called the different stylesheets and calendar div

        ….
        Reply
    krystyna Sep 19, 10:15 am

    This is a really nice example.

    How could I include a background-color to the default day? It currently only has the selection made with a border.

    Thanks.
    Reply

Leave a Reply
* Name
* Email
* Comment
Minimum length: 20 characters
Our Products
Show more

    DESIGN FRAMEWORK
    Startup Framework 2
    $249
    WEBSITE FRAMEWORK
    Slides
    $249
    WORDPRESS PLUGIN
    Qards
    $99
    DESIGN FRAMEWORK
    Flat UI Pro
    $39

Designmodo Market
Show more

    UI KIT
    Chameleon – iOS UI Kit
    $48
    UI KIT
    Portal UI Pack @1x
    $48
    MOCKUPS
    HERO iPhone 7 Plus Mockups
    $28
    UI KIT
    Daily UI Kit
    $34
    UI KIT
    The Pear Starter Web UI Kit
    $28

Newsletter

Get our products/news earlier than others, let’s get in touch.
Sponsors
Free Photos
WordPress Themes
- Advertise With Us -
Popular Posts (Month)

    How to Move a WordPress Website from HTTP to HTTPS/SSL
    How to Move a WordPress Website from HTTP to HTTPS/SSL
    The Ultimate UX Design of: the Credit Card Payment Form
    The Ultimate UX Design of: the Credit Card Payment Form
    15 TED Talks Every Web Designer Should Watch
    15 TED Talks Every Web Designer Should Watch
    Design Stereotypes: Masculine and Feminine Design Techniques
    Design Stereotypes: Masculine and Feminine Design Techniques
    Crazy Sliders – 10 Ways of Taking Sliders to the Next Level
    Crazy Sliders – 10 Ways of Taking Sliders to the Next Level
    Iconshock: Two Million Free Icons Later
    Iconshock: Two Million Free Icons Later
    CaptainForm – A Hero Form Builder
    CaptainForm – A Hero Form Builder
    How to Upload Themes and Plugins on WordPress.com
    How to Upload Themes and Plugins on WordPress.com
    What Typography Means in Email & How to Choose the Best Fonts
    What Typography Means in Email & How to Choose the Best Fonts
    MailOptin Review – The Best WordPress List Building and Automated Newsletters Plugin
    MailOptin Review – The Best WordPress List Building and Automated Newsletters P...

Recent Articles

    Create a Product Page with Interactive Colors in HTML, CSS3 & jQuery
    Create a Product Page with Interactive Colors in HTML, CSS3 & jQuery
    Create a Full-Screen Slider Using HTML, CSS3 and jQuery
    Create a Full-Screen Slider Using HTML, CSS3 and jQuery
    Create a Full-Screen Navigation Menu in CSS3 & jQuery
    Create a Full-Screen Navigation Menu in CSS3 & jQuery
    How to Create Checkout Form Using HTML, CSS3 and jQuery
    How to Create Checkout Form Using HTML, CSS3 and jQuery
    Create a Statistics UI Panel Using HTML & CSS3
    Create a Statistics UI Panel Using HTML & CSS3
    How to Create a Shopping Cart UI using CSS & JavaScript
    How to Create a Shopping Cart UI using CSS & JavaScript
    How to Create a Credit Card UI using HTML and CSS3
    How to Create a Credit Card UI using HTML and CSS3
    How to Create a CSS3 Mega Drop-Down Menu
    How to Create a CSS3 Mega Drop-Down Menu
    How to Create an Upload Form using jQuery, CSS3, HTML5 and PHP
    How to Create an Upload Form using jQuery, CSS3, HTML5 and PHP
    How to Create a Responsive Image Slider in jQuery and CSS3
    How to Create a Responsive Image Slider in jQuery and CSS3

    Contact Us
    About
    Privacy
    Terms
    Advertise
    Affiliates
    Newsletter

    Copyright © 2017 Designmodo. All Rights Reserved.
    Designmodo is a popular web design blog and shop.

We use cookies to personalise content and ads, to provide social media features and to analyse our traffic. We also share information about your use of our site with our social media, advertising and analytics partners.
OkMore Info

