# Based on the "WP-Polls" plugin made by GamerZ

[Check the original proyect on GitHub](https://github.com/lesterchan/wp-polls "https://github.com/lesterchan/wp-polls")
Requires at least: 3.9  
Tested up to: 4.3  
### Development
Stable tag: 2.70  

This plugin is based on the "WP-Polls" plugin made by GamerZ with the main difference that i've removed all the provided CSS files and added a little of extra HTML markup to make it easier for the Developer and the designer for applying custom style.<a href=""></a>
If you want to use your own CSS styles, you just have to create a file called `polls-css.css` inside a folder called `css/` on your `theme directory`. If it doesn't exist, it will look to the same file on your `theme directory` AND if it doesn't exist, it will try to load it from your plugin folder `wp-polls/`.

> Adds an AJAX poll system to your WordPress blog. You can also easily add a poll into your WordPress's blog post/page.

> ### Translations
> [http://dev.wp-plugins.org/browser/wp-polls/i18n/](http://dev.wp-plugins.org/browser/wp-polls/i18n/ "http://dev.wp-plugins.org/browser/wp-polls/i18n/")

### Changelog

### Versión 1.0 (01/08/2015)
* [wp-polls.php]
	* Added `class` & `id` to the poll question tag
	* Added class `.list` to the `.wp-polls-ul`
	* Removed "text-align:center;" from most of the front-end tags
	* Changed the `<p>` tag to `<h3>` on the titltes
	* Added class `.input-row` to the submit container. Also the submit button now has `.wp-poll-submit` as new classname
	* New CSS loading spinner animation
	* New class "wp-poll-view-results" for the link to the poll results
	* Bodoke CSS class on the submit poll button
	* New syntax for the poll answer on the results section
	* Multiple option form now has class `.wp-multi-poll`. The same goes for the single-choice form `.wp-single-poll`
	* New attr "data-max-ans" that set the max answers avaiable for the user to be selected
* [polls-template.php]
	* Added `class` & `id` to the poll question tag
	* Added class `.list` to the `.wp-polls-ul`
	* Removed "text-align:center;" from most of the front-end tags
	* Changed the `<p>` tag to `<h3>` on the titltes
	* Added class `.input-row` to the submit container. Also the submit button now has `.wp-poll-submit` as new classname
	* New class "wp-poll-view-results" for the link to the poll results
	* Bodoke CSS class on the submit poll button
	* New syntax for the poll answer on the results section
* [polls-css.css]
	* Removed from the plugin directory
	* WP-Polls will search not only in your theme's directory, it will also look inside a custom `css/` folder inside your theme`s directory
* [polls-css-rtl.css]
	* Deprecated. Everything you need it's inside `polls-css.css`
* [polls-js.dev.js]
	* Using this file insted of `poll-js.js`
	* New function that adds a `.checked` class to the label next to the `input:checked`