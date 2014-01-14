=== Join My Multisite ===
Contributors: Ipstenu
Tags: multisite, wpmu, registration, users
Requires at least: 3.4
Tested up to: 3.5
Stable tag: 1.1
Donate link: https://store.halfelf.org/donate/

Allow site admins to automatically add existing users to their site, or let users decide at the click a button.

== Description ==

When you want to add a user to every site on your network, you've got some pretty cool plugins for that as a network admin. But sometimes you want to let your site-managers have that control, and sometimes you want to make it optional.

By activating this plugin, you give your Site Admins the following options:

* Auto-add users
* Have a 'Join This Site' button in a widget
* Keep things exactly as they are
* Create a per site registration page

It's really that simple! 

If they decide to auto-add, then any time a logged in user visits a site, they will be magically added to that site. If they decide to use a 'Join This Site' button, then they can customize the button message text for users who are logged in but not members, not logged in, or already members. Don't worry, if you have registation turned off, they won't see the 'register' button.

When you have registration turned on, each site can chose to use 'Per Site Registration,' which will allow them to create a page on their site just for registrations and signups. To display the signup code, just put <code>[join-my-multisite]</code> on the page.

* [Plugin Site](http://halfelf.org/plugins/join-my-multisite/)
* [Donate](https://store.halfelf.org/donate/)

==Changelog==

= 1.1 =
12 October, 2012 by Ipstenu

* Added in a per-site registration page option.
* Corrected bug where non-network admins couldn't make changes

=  1.0 =
07 October, 2012 by Ipstenu

* First completed version.

== Installation ==

This plugin is only network activatable. Configuration is done per-site via a page in the 'Users' section.

== Screenshots ==

1. Menu
1. Widget
1. Sample per-site registration front end

== Upgrade Notice ==

None yet.

== Frequently Asked Questions ==

= What happens if the network doesn't allow registrations? =

If registration is turned off, the widget won't display anything for logged-out users.

The <code>[join-my-multisite]</code> shortcode will display a notice that registration is unavailable.

= How do I use the per-site registration page? =

<em>None of this will work if the Network Admin has not enabled registrations.</em>

First make a page for your registration. You can name it anything you want, however you can only use top-level pages (so domain.com/pagename/ and not domain.com/parentpage/childpage/). On that page, enter the shortcode <code>[join-my-multisite]</code> around any other content you want.

Next, go to Users > Join My Multisite and check the box to allow for Per Site Registration. Once that option is saved, a new dropdown will appear that will let you select a top-level page on your site. Select which page, and you are good to go.

= If I use the per-site registration, do I have to use the widget? =

Nope! In fact, you can even select 'none' (i.e. leave things as they are) and <em>still</em> use the per-site shortcode, because magic.

= What if the network allows registration and I don't make a site page? =

Then non-logged-in users will be redirected to the network registration page, and they may not be automatically added to your site (I'm working on that). I strongly suggest you create a page.

= How do I style the button? =

By default it will pick up whatever style your theme has, so if it styles buttons, you'll automatically match. If you want more, the css is `input#join-site.button` to play with the button.

= How do I style the per-site registration page? =

In your theme's CSS. This is basically the default WordPress signup page, just done in short-code form, so it will default to use your site's CSS anyway. The css falls under `.mu_register` of you want to override it in your theme.

= Can users sign up for a blog and an account when using the shortcode? =

No. That's such a massive network thing, the tinfoil hat in me didn't want to do it. You could fiddle with the signup page code, if you wanted, but I don't plan to support it.