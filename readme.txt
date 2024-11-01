=== WP Verify API ===
Contributors: anorouzi
Tags: OTP, email verification, verify email, One-time password, Verify API
Requires at least: 4.6.1
Requires PHP: 5.4
Tested up to: 5.4.1
Stable tag: 1.0.3
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Generate and check verification code by WP API

== Description ==

NOTICE : This plugin is used by WordPress developers and can be a bit confusing for beginner WordPress users.

This plugin generates a verification code via WordPress API and sends it to the specified email.
You can then check the code entered by the user with the API.

= Docs & Support =

** Generate verification code **

`example.com/wp-json/wva/v1/email`

Email should be post in JSON format.
Example :`{"email" : "anorouziiii@gmail.com"}`

** Check verification code **

`example.com/wp-json/wva/v1/verify`

Email and verification code should be posted in JSON format. if the code is correct and the expire time is not reached, it will return `true` otherwise it's `false` then you can do whatever you want with the result like for OTP, Email Owner verification, and so on.
Example :`{"email" : "anorouziiii@gmail.com","verify" : "53737"}`

= Features =
*   API-Based system for generating and check code.
*   Customize expiration time for code.
*   Customize code digits


== Installation ==

1. Upload the 'wp-verify-api' folder to the '/wp-content/plugins/' directory
1. Activate the WP Verify API plugin through the 'Plugins' menu in WordPress
1. You can change the plugin settings from Settings > WP Verify API menu


= 1.0.0 =
* Initial release.