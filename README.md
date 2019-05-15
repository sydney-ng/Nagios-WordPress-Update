Nagios-WordPress-Update
===============

This script is a modified version of the original wp-version.php written by @jinjie. 
Original [here](http://exchange.nagios.org/directory/Plugins/CMS-and-Blog-Software/Wordpress/check_wp_version/details)

__Purpose:__
- Data that may be not as relevant for the purpose of monitoring if WordPress is updated is is filtered out. 
- Currently, any updates will be marked as 'Critical' for Theme and and Plugins. However, since is the responsiblity of the departments to update these features, this is data that can be made note of, but should not be counted towards the number of 'Critical' errors that are used as the base metrics for the website.
- We therefore have grouped theme and plugin updates into one category and only using them to count as 'Warnings' and not 'Critical'. 
