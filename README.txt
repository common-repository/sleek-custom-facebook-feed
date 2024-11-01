=== Custom Facebook Feed ===
Contributors: sleekplugins
Tags: Facebook, Facebook feed, Facebook posts, Facebook wall, Facebook events, Facebook page, Facebook group, Facebook fans, Facebook likes, Facebook followers, Face book, Facebook pages, Facebook Like Box, Facebook plugin, Facebook walls, custom, customizable, seo, responsive, mobile, social media
Requires at least: 3.0
Tested up to: 4.6
Stable tag: 2.4.4
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

The Custom Facebook Feed allows you to display completely customizable Facebook feeds of any public Facebook page or group on your website

== Description ==

Display a **completely customizable**, **responsive** and **search engine crawlable** version of your Facebook feed on your website. Completely match the look and feel of the site with tons of customization options!

= Features = 

* **Completely Customizable** - By default the Facebook feed will adopt the style of your website, but can be completely customized to look however you like - with tons of styling and customization options!
* Facebook feed content is **crawlable by search engines** adding SEO value to your site - other Facebook plugins embed the feed using iframes which are not crawlable
* Completely **responsive** and mobile optimized - layout looks great on any screen size and in any container width
* Display **feeds from multiple different Facebook pages/groups** and use the shortcode to embed them into a page, post or widget anywhere on your site
* Show **events** from your Facebook feed with name, date/time, location and description
* Add your own **custom CSS**
* **Caching** means that your Facebook posts load lightning fast. Set your own caching time - check for new posts on Facebook every few seconds, minutes, hours or days. You decide.
* **Super simple to set up**. Just enter your Facebook page ID and you're done.
* Show and hide certain parts of each Facebook post
* Show or hide the Facebook profile picture and name of the author above each post
* Display Facebook posts by just the page owner, everyone who posts on your Facebook page, or only other people
* Control the width, height, padding and background color of your Facebook feed
* Customize the size, weight and color of text
* Choose to set a background color and rounded corners on your Facebook posts
* Supports Facebook tags - creates links when using the @ symbol to tag people in your Facebook posts
* Automatically links hashtags used in posts to the hashtag page on Facebook
* Select the number of Facebook posts to display
* Select from a range of date formats or enter your own
* Use your own custom link text in place of the defaults
* Use the shortcode options to style multiple Facebook feeds in completely different ways
* Set a maximum character length for both the text and descriptions of your Facebook posts
* Create a customizable header with a range of icons for your Custom Facebook Feed
* Localization/i18n support to allow every part of the feed to be displayed in your language


= Benefits =

* **Increase social engagement** between you and your users, customers, fans or group members
* **Save time** by using the Custom Facebook Feed to generate dynamic, search engine crawlable content on your website
* **Get more likes** by displaying your Facebook content directly on your site
* **Improve your SEO** as all of that quality keyword-rich Facebook content from posts and comments is directly embedded into your website
* Display your Facebook content your way to perfectly match your website's style
* The plugin is **updated regularly** with new features, bug-fixes and Facebook API changes
* Support is quick and effective
* We're dedicated to providing the **most customizable**, **robust** and **well supported** Facebook feed plugin in the world!

[View the reviews](http://wordpress.org/support/view/plugin-reviews/custom-facebook-feed) to see what other users are saying about the Custom Facebook Feed plugin.

== Installation ==

1. Install the Custom Facebook Feed either via the WordPress plugin directory, or by uploading the files to your web server (in the `/wp-content/plugins/` directory).
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Navigate to the 'Facebook Feed' settings page to configure your feed.
4. Use the shortcode `[custom-facebook-feed]` in your page, post or widget to display your feed.
5. You can display multiple feeds of different Facebook pages by specifying a Page ID directly in the shortcode: `[custom-facebook-feed id=sleekplugins num=5]`.


= How do I find the Page ID of my Facebook page or group? =

If you have a Facebook **page** with a URL like this: `https://www.facebook.com/sleekplugins` then the Page ID is just `sleekplugins`. If your page URL is structured like this: `https://www.facebook.com/pages/sleekplugins/123654123654123` then the Page ID is actually the number at the end, so in this case `123654123654123`.


= Are there any limitations on which Facebook page or group feeds I can display? =

The Facebook feed you're trying to display has to be from a publicly accessible Facebook page or group. This means that you can't display the feed from your own personal Facebook profile or private Facebook group. This is to do with Facebook's privacy policies. You can't display a non-public Facebook feed publicly.

If your Facebook page has any restrictions on it (age, for example) then it means that people have to be signed into Facebook in order to view your page. This isn't desirable for most Facebook pages as it means that it isn't accessible by people who don't have a Facebook account and that your Facebook page can't be crawled and indexed by search engines.

An easy way to determine whether your Facebook page is set to public is to sign out of your Facebook account and try to visit your page. If Facebook forces you to sign in to view your page then it isn't public. You can change your Facebook page to public in your Facebook page settings simply by removing any age or location restrictions you have on it, which will then allow the Custom Facebook Feed plugin to access and display your feed.

= Can I display feeds from multiple Facebook pages or groups? =

You can set your default Facebook Page ID on the Custom Facebook Feed settings page within the WordPress admin, you can then define different page IDs in the shortcodes you use to show multiple feeds from different Facebook pages. Just use the id option in your shortcode like so: [custom-facebook-feed id=another_page_id]. You can use as many shortcodes as you like with as many different IDs as you like.

= Can I display the feed from a personal Facebook profile? =

Due to Facebook's privacy policy you're not able to use the plugin to display all of your posts from a personal profile, only from a public page or group, as posts from a personal profile are protected for privacy reasons. You may have limited success in displaying certain posts from a personal profile but most posts are not able to be displayed.

If you're using the profile to represent a business, organization, product, public figure or the like, then we'd advise converting your profile to a page per [Facebook's recommendation](http://www.facebook.com/help/175644189234902/), as there are many advantages to using pages over profiles.

Once you've done so, the plugin will be able to retrieve and display all of your posts.


= Is the content of my Custom Facebook Feed crawlable by search engines? =

It sure is. Unlike other Facebook plugins which use iframes to embed your Facebook feed into your page once it's loaded, the Custom Facebook Feed uses PHP to embed your Facebook feed content directly into your page. This adds dynamic, search engine crawlable content to your site.

= How do I embed the Custom Facebook Feed directly into a WordPress page template? =

You can embed your Facebook feed directly into a template file by using the WordPress [do_shortcode](http://codex.wordpress.org/Function_Reference/do_shortcode "WordPress.org do_shortcode reference") function: `<?php echo do_shortcode('[custom-facebook-feed]'); ?>`.


= Create a basic slideshow from your Facebook posts =

The Custom Facebook Feed plugin doesn't currently have a slideshow feature built into it, but it's possible to achieve a basic slideshow by doing the following:

1) Add a class to the shortcode of the Facebook feed that you want to convert into a slideshow:

`[custom-facebook-feed class="slideshow"]`

2) Set the number of posts to display to be the number of Facebook posts you want to include in the slideshow (10 for example). You can do this by using the `num` shortcode option:

`[custom-facebook-feed class="slideshow" num=10]`

3) Add the following to the plugin's **Custom JavaScript** section, which is under the 'Misc' tab on the plugin's 'Customize' page. Please note, if you change the class option in the shortcode above to be anything but "slideshow" then make sure to change that on the first line of the snippet below:

`var shortcodeClass = 'slideshow',
    cffSpeed = 5000, 
    $cff = $('#cff.'+ shortcodeClass);
    $cffItem = $cff.find('.cff-item'),
    cffNum = $cffItem.length,
    cffCur = 0;
$cffItem.hide();
setTimeout(function(){ $cff.find('.cff-item').eq(0).show(); }, 200);
setInterval(function(){
    $cff.find('.cff-item').eq(cffCur).fadeOut( "fast", function() {
        if( cffCur == cffNum-1 ) cffCur = -1;
        cffCur++;
        $cff.find('.cff-item').eq(cffCur).fadeIn();
    });
}, cffSpeed);`

4) You can change the speed of the transition by editing the **cffSpeed = 5000** value at the top of the snippet. 5000 is equal to 5 seconds (5000ms).


= My Facebook feed appears to have stopped updating / working =

If your Facebook feed doesn't appear to be showing the most recent Facebook posts then the most likely explanation is that the recent Facebook posts in your feed may be shared from a user's personal Facebook profile. Facebook's privacy policy doesn't allow posts that you share from personal Facebook profiles to be shared outside of Facebook as the posts don't technically belong to your Facebook page, they belong to the user who posted it to their personal Facebook profile. 

Please note, this isn't a limitation of our plugin, it's a restriction which Facebook places on it's content in order to protect the privacy of their Facebook users.

**Potential solutions**

* You could re-post the Facebook post to your page rather than sharing it to your Facebook page. If you re-post the content as your own post on your Facebook page then the content now originates from your Facebook page and will be displayed in the Facebook feed on your website.

* If you were to share a post from another Facebook page or public source, rather than sharing it from someone's personal Facebook profile, then it would show up in your feed outside of Facebook, but by default any posts that originate from a personal Facebook profile are protected by Facebook's privacy policy and is the private content of that Facebook profile owner.

= How do I customize my Facebook feed? =

You can customize the Facebook feed by setting the options on the Customize page, which can be found under the Facebook Feed menu in your left hand WordPress admin menu. If you need even deeper customization than the built in options allow then you can add your own CSS to the plugin in the Custom CSS section under the Misc tab to further customize your Facebook feed.

You can also override these styles for individual Facebook feeds by setting options within the shortcode. For example, you can change the height of a specific Facebook feed like so: `[custom-facebook-feed height=500px]`.

= The Custom Facebook Feed shortcode options aren't working =

The most common causes of this are:

1) There's HTML tags within the [custom-facebook-feed] shortcode which are preventing it from working correctly

If you copied and pasted the shortcode into the Visual editor on your WordPress page/post editor then it may have inadvertently included some HTML tags from the page that you copied it from. The easiest way to check this is to view the 'Text' view in your WordPress editor and see whether there are any stray HTML tags in the shortcode itself.

2) The shortcode includes curly single quote characters

If your shortcode includes single quotes then check that they are the standard single quotes and not the curly kind.

3) Typo in the shortcode option

Ensure that there aren't any spelling errors in the shortcode options that you're using and that the format is consistent with that demonstrated on the [Shortcode Options reference page](http://sleekplugins.com/facebook-plugins/shortcodes/ "The shortcode options aren't working").

= Facebook avatar pictures aren't showing up in my Facebook feed =

The most common reason for this is that an add-on or extension you have installed in your web browser is blocking the pictures being loaded from Facebook. Try checking to see whether you have any add-ons or extensions installed in your browser and, if so, try disabling them to see whether that solves the problem and displays the pictures from Facebook.


= Why do I need the Custom Facebook Feed plugin? =

**Increase Social Engagement**
Increase engagement between you and your users, customers, fans or group members. Get more Facebook likes by displaying your Facebook content directly on your site.

**Save Time**
Don't have time to blog? Save time by using the Custom Facebook Feed instead to generate dynamic content for your website.

**Display Your Facebook Content Your Way**
Tailor your Facebook feeds to display whatever types of content you like. Integrate your Facebook content into your website to completely match the look and feel of the site. No more uncustomizable Facebook iframes.

**Add Dynamic SEO Facebook Content to Your Site**
All of that quality keyword-rich Facebook content from Facebook posts is directly embedded into your website.

**No Coding Required**
Choose from tons of built-in customization options to create a truly unique feed of your Facebook content.

**Mind-blowing Customer Support**
We understand that sometimes you need help, have issues or just have questions. We love our customers and strive to provide the best support experience in the business. If you need support then just let us know and we'll get back to you right away.

= How to get a Facebook Access Token =

You no longer need your own Access Token to use the Custom Facebook Feed Plugin, but if you'd like to use your own then you will need to obtain one from Facebook.  Don't worry though, this is really easy to do.  Just follow the steps below:

**1)** Go to [developers.facebook.com](http://developers.facebook.com "Facebook developers website") and click on Log In in the top right.  Log in using your personal Facebook credentials.

**Note:** The personal Facebook account that you use to register as a Facebook developer does not need to be associated in any way with the Facebook page or Facebook group whose posts you want to display. You can use the Facebook Access Token you receive to display the Facebook posts from any public Facebook page or open Facebook group.

**Note:** You cannot log in to the Facebook Developer site using a Facebook Page or Facebook Business account. You must use the username and password from your personal Facebook profile. Facebook doesn't allow businesses to register as Facebook developers, only individuals.

**2)** If this is your first time signing in to the Facebook Developer portal then click on Register Now. Registering is a quick an easy process which will take less than a couple of minutes.  If you're already registered as a Facebook developer then you can skip ahead to step 9.

**3)** Accept the Facebook terms and click Continue.

**4)** Enter your phone number to confirm your account.

**5)** Facebook will send you an automated text message containing a confirmation code. Enter it in the box and click Confirm.

**6)** Choose to share your phone number with Only Me (unless you wish to share it with publicly or with Facebook friends).

**7)** You can skip the next step by clicking Skip.

**8)** Click Done.
 
**9)** Now click on Create New App.

**10)** Enter your Facebook App Name. This can be anything you like. Click Continue.

**11)** Fill in Facebook's Security Check and click Continue.

**12)** Your Facebook App should now be set up. Copy and paste your Facebook App ID and Facebook App Secret into the fields.

= What some of our users think =

= The Importance of Facebook for Small Businesses =

**Below is an article indicating the importance of building a Facebook community around your business or product. The Custom Facebook Feed plugin can help you to build a Facebook community more easily and effectively.**

A few years back when Mark Zuckerberg came up with his concept of a social networking site and named it Facebook, he had no idea what it would become in the time to come. Facebook has quite literally revolutionized the way we look at social networking. With over 700 million active Facebook users, it is definitely the biggest platform you can get if you seek to engage with many people simultaneously. Though Facebook is the premiere social networking platform, it also holds a lot of potential for businesses. The fact that Facebook can help businesses in growing and reaching out to a new customer base has added to Facebook's popularity.

Today when you look at Facebook and the Facebook groups or Facebook pages that exist on the site, you will find that every popular brand is there. They are not only there but are active on Facebook on almost a daily basis. For the present generation, who spend a lot more time on the internet than on the TV, brands needed to change their approach. Facebook provides the best possible solution in this scenario. However, it is not only the big brands that make the full use of Facebook's social media power. Even small businesses can benefit greatly from using Facebook if they make optimal use of the various features that Facebook has to offer.

**Why Use Facebook for Your Business?**

When you start your business, many things have to be taken into account. Amongst the tons of seemingly more important things, you might question the need for using Facebook. Often people end up feeling that Facebook is too trivial a task and can be accomplished at anytime. Here are some reasons why you should have your presence on a social networking giant like Facebook and take it very seriously:

Customer Interaction: Having your business on Facebook through a Facebook fanpage or a Facebook group is a great way to learn more about your customers. Through Facebook comments or Facebook posts, you get to have direct feedback and conversations with your target audience on Facebook. The people who like your Facebook fanpage or join your Facebook group are only there because they want to be. They are there to know what they can about you and you can do the same thing.

Give a personal touch to your business: Being well connected is important for any business, especially for a small one. You need to be able to communicate with people and grow your contacts. The best possible way to do that is through direct involvement. Facebook allows you to give your business an image and then you can actually have live conversations with people who matter, making communicating through Facebook a more personal experience then what you get on a TV.

Develop a loyal fan base: Facebook allows you to develop your very own Facebook community. All you need to do is, post links and content that is both relevant and useful. You can even have promotional Facebook campaigns and Facebook contests through your Facebook page and offer incentives as well. If done correctly, you will find that you can develop a loyal community for your business on Facebook.

SEO: Search Engine Optimization is a key aspect for anyone who wants to build a significant presence on the web. Having a Facebook page for your business can help you in your SEO efforts as well. All the links and Facebook posts on the page are indexed by search engines. So having a Facebook page flowing with continuous relevant content will definitely give you a jump in search engine rankings.

Beat your competition: One of the biggest reasons for you to make sure that you are on Facebook is that your competition might already be there. In this cut throat environment, lagging behind will make it really hard for your business to succeed.

Viral promotion: If someone ends up liking your page then it appears in their Facebook news feed. This makes it possible for your business to be in their eyes on a regular basis through Facebook status updates or content posting. What's more, if they comment on your Facebook post, their Facebook friends will also see your Facebook post and this will help in viral promotion of your business.

Facebook Ads: Your business at Facebook is not just limited to a Facebook page or Facebook group. Facebook also offers you a chance to put up Facebook advertising campaigns. You can build your Facebook advertisements, and as per your budget requirements, go for a Facebook campaign suitable for your business. You can also choose the set of people to whom these Facebook ads will be visible. You can target your Facebook ads on the basis of demographics, educational level, interests etc. It is also up to you to decide how often these Facebook ads will appear.

Save money: Apart from these facts, Facebook is free. You do not need to spend anything for promoting your company through a Facebook page. Facebook already has people addicted to it. This means you do not have to look for customers – they are already there on Facebook.

**How to Make the Best Use of Facebook?**

Many people feel that simply having a Facebook page or Facebook group is enough to help their company. It cannot be further from the truth. In fact, if you are not going to use it properly, then it can be more disadvantageous than not being on Facebook.

Make sure that you do not leave your Facebook page or Facebook group after a few days. It reduces participation and gives your business a bad name. Do not spam through your Facebook pages, it is the simplest way to lose customers. Make sure that your Facebook fans and members are rewarded for being there in your Facebook group or Facebook page. You could give them free coupons via Facebook or something similar.

Facebook has really changed the way people go about promoting their business. With so many people with varied interests available on a single platform, there is something for everyone. All you need to do is find the right target audience and then market your business to them. Facebook provides you all the tools required to reach these people.

Credit iMarketing Factory - "The Importance of Facebook for Small Businesses"

== Screenshots ==

1. By default the Facebook feed inherits your theme's default styles and is completely responsive
2. Completely customize the way your Facebook feed looks to perfectly match your site
3. Use custom CSS to customize every part of the Facebook feed
4. Display Facebook events
5. Configuring the Custom Facebook Feed plugin
6. General options - Custom Facebook Feed Layout & Style page
7. Typography options - Custom Facebook Feed Layout & Style page
8. Misc options - Custom Facebook FeedLayout & Style page
9. It's super easy to display your Facebook feed in any page or post