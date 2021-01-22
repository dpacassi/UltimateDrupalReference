[![GitHub last commit](https://img.shields.io/github/last-commit/dpacassi/UltimateDrupalReference.svg)](https://github.com/dpacassi/UltimateDrupalReference)
[![GitHub contributors](https://img.shields.io/github/contributors/dpacassi/UltimateDrupalReference.svg)](https://github.com/dpacassi/UltimateDrupalReference)
[![license](https://img.shields.io/github/license/dpacassi/UltimateDrupalReference.svg)](https://github.com/dpacassi/UltimateDrupalReference/blob/master/LICENSE)
[![Twitter URL](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&logo=twitter)](https://twitter.com/intent/tweet?text=Starting+with+%23Drupal%3F+Or+simply+just+stuck%3F+Have+a+look+at+the+%23UltimateDrupalReference+on+https%3A%2F%2Fgithub.com%2Fdpacassi%2FUltimateDrupalReference%2C+it+might+help+you+out%21)

# Ultimate Drupal Reference
When it comes to [Drupal](https://www.drupal.org/), there are a lot of videos, blog posts and general how-to's out there.  
While some of them are good, others are in need of improvement and a few of them are simply outdated.

This project will try to list you the **best, most promising and most efficient** resources that you might need when developing a Drupal site.  

## Contribution guidelines
This project lives through new and up-to-date resources from the community, from **you**!  
If you would like to add a resource or contribute in any other kind of way, be sure to read our [contribution guidelines](CONTRIBUTING.md).

## Table of contents
- [Installing Drupal](#installing-drupal)
  - [Evaluate Drupal projects without installing Drupal](#evaluate-drupal-projects-without-installing-drupal)
  - [Drupal requirements](#drupal-requirements)
  - [Official installation page](#official-installation-page)
  - [Drupal VMs](#drupal-vms)
  - [Composer](#composer)
  - [Drupal CLI's](#drupal-clis)
  - [IDE's](#ides)
- [Site building with Drupal](#site-building-with-drupal)
- [Theming in Drupal](#theming-in-drupal)
- [Distributions](#distributions)
- [Modules](#modules)
  - [Commerce](#commerce)
  - [Content](#content)
  - [Developer tools](#developer-tools)
  - [Forms](#forms)
  - [Media](#media)
  - [Migration](#migration)
  - [Multilingualism](#multilingualism)
  - [Multisite](#multisite)
  - [Performance](#performance)
  - [SEO / Analytics](#seo--analytics)
  - [Security](#security)
  - [Site building](#site-building)
  - [Site navigation](#site-navigation)
  - [Social media](#social-media)
  - [User & Roles management](#user--roles-management)
  - [Views](#views)
- [Themes](#themes)
  - [Frontend themes](#frontend-themes)
  - [Admin themes](#admin-themes)
- [Troubleshooting](#troubleshooting)
  - [Update to the latest stable release](#update-to-the-latest-stable-release)
  - [Read the project's description](#read-the-projects-description)
  - [Issue queue](#issue-queue)
  - [Drupal Answers](#drupal-answers)
  - [Google](#google)
  - [IRC / Slack support](#irc--slack-support)
- [Contributing to Drupal](#contributing-to-drupal)
- [Video tutorials](#video-tutorials)
  - [Beginner training series](#beginner-training-series)
  - [General](#general)
  - [Modules](#modules-1)
  - [Theming](#theming)
- [Blog posts](#blog-posts)
- [Further resources](#further-resources)
- [Drupal PaaS](#drupal-paas)
- [Get in touch with the Drupal community](#get-in-touch-with-the-drupal-community)
- [Credits](#credits)
- [License](#license)

## Installing Drupal
There are different ways of installing Drupal.
You can either install it directly on your local machine (or any server) or you can also work with a VM if you prefer.  
If you really just want to catch a *quick glimpse* about a specific Drupal distribution, module or theme, then you don't even
need to install anything! Check out the next section for details.

If you want to run Drupal locally (and directly) on your Mac machine, check out this [great tutorial](https://getgrav.org/blog/macos-mojave-apache-multiple-php-versions).

### Evaluate Drupal projects without installing Drupal
No further information needed. Simply visit [simplytest.me](https://simplytest.me/) and launch your custom sandbox!

### Drupal requirements
In order to be able to run Drupal on your machine (or any server), you need a web server with PHP and a SQL database server.
Please check the [official requirements page](https://www.drupal.org/docs/8/system-requirements) for more details.

### Official installation page
Up-to-date and detailed instructions can be found on the [official installation page](https://www.drupal.org/docs/8/install).

### Drupal VMs
If you prefer working with a VM, check out following alternatives:
- [Docker](https://hub.docker.com/_/drupal/)
- [Drupal VM](https://www.drupalvm.com/)

### Composer
While not required, it's **highly recommended** that you set up your Drupal project with [Composer](https://getcomposer.org/),
regardless of your technical setup.  
Check the [Composer template for Drupal projects](https://github.com/drupal-composer/drupal-project) to install Drupal quickly via Composer.

#### Composer prestissimo
If you want to speed up Composer, have a look at [prestissimo](https://github.com/hirak/prestissimo).  
You can install it globally (no project dependency) to speed up Composer installations by a lot!  
Simply run `composer global require hirak/prestissimo` and you're good to go.  
Read more about prestissimo in its [project page](https://github.com/hirak/prestissimo).

### Converting a non-Composer Drupal codebase to use Composer
Jeff Geerling wrote a nice [blog post](https://www.jeffgeerling.com/blog/2018/converting-non-composer-drupal-codebase-use-composer) about
convertig a non-Composer Drupal codebase to use Composer.  
Check it out and benefit from Composer!

### Drupal CLI's
When it comes to developing custom modules, themes or simply automate certain tasks with scripts/cronjobs, there are two
major Drupal CLI's which can be a huge help for you:
- [Drupal Console](https://drupalconsole.com/)
- [Drush](http://www.drush.org/)

## IDE's
There are lots of different IDE's and editors for PHP. But *most* Drupal developers tend to use [PhpStorm](https://www.jetbrains.com/phpstorm/).  
Do you use any other IDE or editor? Please let me know!

## Site building with Drupal
Once you have Drupal set up and running, it's time for site building.  
Have a look at the great documentation on drupal.org about [site building](https://www.drupal.org/site-building)
as well as as understanding the [concepts of Drupal](https://www.drupal.org/docs/8/understanding-drupal-8/overview).

## Theming in Drupal
- [Twig Documentation](https://twig.symfony.com/doc/2.x/) - Twig is the templating language used in building a Drupal 8 Theme
- [Debugging Twig Templates](https://www.drupal.org/docs/8/theming/twig/debugging-twig-templates) - This will allow you to see which templates are in use on a page, which template is used to render each item on the page, any hooks for that template, and give you suggestions for naming your new templates
- [Drupal 8 Theming Fundamentals, Part 1](https://www.lullabot.com/articles/drupal-8-theming-fundamentals-part-1) and [Part 2](https://www.lullabot.com/articles/drupal-8-theming-fundamentals-part-2) - An overview of creating and working in a Drupal 8 theme
- [Drupal.org Theming Guide for Drupal 8](https://www.drupal.org/docs/8/theming) - The official guide to Drupal 8 theming. Not always the easiest to understand but very helpful for reference on many topics.

## Distributions
While Drupal 8+ core comes with lots of functionality already, the strength of Drupal lies in its extensibility.  
Distributions are full copies of Drupal that include Drupal Core, along with additional software such as themes, modules, libraries, and installation profiles.  
They're handy if you *really* just want to have a quick start with Drupal.
- [Druppio](https://www.drupal.org/project/druppio_small_business_distribution) - A small business distribution with demo content.
- [Lighting](https://www.drupal.org/project/lightning) - Lightning is a solid Drupal starter kit that enables developers to create great authoring experiences and empower editorial teams.
- [Open Social](https://www.drupal.org/project/social) - Open Social is a out of the box solution for online communities.
- [Thunder](https://www.drupal.org/project/thunder) - Thunder is a Drupal 8 distribution for professional publishing.
- [Varbase](https://www.drupal.org/project/varbase) - Varbase is an enhanced Drupal distribution packed with adaptive functionalities and essential modules, that speed up your development, and provides you with standardized configurations.
- .. and many more on [drupal.org](https://www.drupal.org/project/project_distribution)

## Modules

### Commerce
- [Drupal Commerce](https://www.drupal.org/project/commerce) - Drupal Commerce is used to build eCommerce websites and applications of all sizes.
  - Also make sure to check out the [commerce documentation](https://docs.drupalcommerce.org/).

### Content
- [Address](https://www.drupal.org/project/address) - Provides functionality for storing, validating and displaying international postal addresses.
- [Automatic Entity Label](https://www.drupal.org/project/auto_entitylabel) - Automatic Entity Label is a small and efficient module that allows hiding of entity label fields. To prevent empty labels it can be configured to generate the label automatically by a given pattern.
- [Corresponding Entity References](https://www.drupal.org/project/cer) - CER keeps reference fields in sync. If you have two entities that refer to each other using Entity Reference (or some other kind of reference field), it saves you the trouble of double-editing your entities in order to have them point at each other.
- [Default Content for D8](https://www.drupal.org/project/default_content) - The Default content module gives your module and install profile a way to ship default content as well as configuration.
- [Diff](https://www.drupal.org/project/diff) - This module adds a tab for sufficiently permissioned users. The tab shows all revisions like standard Drupal but it also allows pretty viewing of all added/changed/deleted words between revisions.
- [Disable Messages](https://www.drupal.org/project/disable_messages) - Gives a site owner options to disable specific messages shown to end users.
- [D8 Editor Advanced link](https://www.drupal.org/project/editor_advanced_link) - Enhances the link Dialog in D8 CKEditor.
- [Entity Clone](https://www.drupal.org/project/entity_clone) - This module add a new entity operation which allows to clone many of the entities (config & content) provided by the Drupal core.
- [Entity Redirect](https://www.drupal.org/project/entity_redirect) - Adds a configurable redirect after saving a node or other entity. The redirect is configurable per bundle.
- [External Links](https://www.drupal.org/project/extlink) - External Links is a small module used to differentiate between internal and external links.
- [Field Formatter Class](https://www.drupal.org/project/field_formatter_class) - Allows site administrators to add classes to the outer HTML wrapper for any field display, so that CSS and Javascript can target them.
- [Iframe](https://www.drupal.org/project/iframe) - A custom field, which lets you add a complete iframe to your content types; including Src-URL, setting width and height, optionally a title above, and optionally a target attribute.
- [Image formatter link to image style](https://www.drupal.org/project/image_formatter_link_to_image_style) - This module provides an additional formatter for image core field, to link to an image style.
- [Office Hours](https://www.drupal.org/project/office_hours) - Defines a 'weekly office hours' field type, allowing you to specify when a location is open or closed.
- [Quick Node Clone](https://www.drupal.org/project/quick_node_clone) - Quick Node Clone is meant as a way in Drupal 8 to clone nodes. It currently supports cloning of most field types including Inline Entity Form and Field Collection.
- [Scheduled Updates](https://www.drupal.org/project/scheduled_updates) - The Scheduled Updates module allows scheduling updates at a specific date and time to entities such as Content(nodes), Users, Terms, Files and many more.
- [Scheduler](https://www.drupal.org/project/scheduler) - Scheduler gives content editors the ability to schedule nodes to be published and unpublished at specified dates and times in the future.
- [State Machine](https://www.drupal.org/project/state_machine) - Provides code-driven workflow functionality. It's also being used in Drupal Commerce to define checkout workflows.
  - This blog post is very helpful to get started with State Machine: [Set up workflows with State machine on Drupal 8](https://www.flocondetoile.fr/blog/set-workflows-state-machine-drupal-8).
- [Voting API](https://www.drupal.org/project/votingapi) - VotingAPI helps developers who want to use a standardized API and schema for storing, retrieving and tabulating votes for Drupal content.

### Developer tools
- [Config Ignore](https://www.drupal.org/project/config_ignore) - This module is a tool to let you keep the configuration you want, in place.
- [Configuration Split](https://www.drupal.org/project/config_split) - Enables you to create different configuration sets for a site.
- [Devel](https://www.drupal.org/project/devel) - A suite of modules containing fun for module developers and themers.
- [Environment Indicator](https://www.drupal.org/project/environment_indicator) - This module will help you to keep sane while working on your different environments by adding a configurable color bar to each one of your environments.
- [Hacked!](https://www.drupal.org/project/hacked) - This module scans the currently installed Drupal, contributed modules and themes, re-downloads them and determines if they have been changed.
- [Stage File Proxy](https://www.drupal.org/project/stage_file_proxy) - Stage File Proxy saves you time and disk space by sending requests to your development environment's files directory to the production environment and making a copy of the production file in your development site.

### Forms
- [Antibot](https://www.drupal.org/project/antibot) - Antibot is an extremely lightweight module designed to eliminate robotic form submissions on your website in an innovative-fashion.
- [Better Login](https://www.drupal.org/project/betterlogin) - Fancy and extendable login forms for Drupal.
- [CAPTCHA](https://www.drupal.org/project/captcha) - A CAPTCHA is a challenge-response test most often placed within web forms to determine whether the user is human.
- [Chosen](https://www.drupal.org/project/chosen) - Chosen uses the Chosen jQuery plugin to make your `<select>` elements more user-friendly.
- [Client-side hierarchical select](https://www.drupal.org/project/cshs) - A simple client-side hierarchical select widget for taxonomy terms.
- [Clientside Validation](https://www.drupal.org/project/clientside_validation) - This module adds clientside validation to all forms and webforms.
- [Form Placeholder](https://www.drupal.org/project/form_placeholder) - This module creates the possibility to quickly add placeholders to all textfields of any form on the site.
- [Honeypot](https://www.drupal.org/project/honeypot) - Honeypot uses both the honeypot and timestamp methods of deterring spam bots from completing forms on your Drupal site.
- [Prepopulate](https://www.drupal.org/project/prepopulate) - The Prepopulate module allows fields in most forms to be pre-populated from the $_REQUEST variable.
- [reCAPTCHA](https://www.drupal.org/project/recaptcha) - Uses the Google reCAPTCHA web service to improve the CAPTCHA system. It is tough on bots and easy on humans.
- [Smart Date](https://www.drupal.org/project/smart_date) - This module attempts to provide a more user-friendly date field, by upgrading the functionality of core in a number of ways.
- [Spam Master](https://www.drupal.org/project/spammaster) - Spam Master protects Drupal based websites from millions of known spam emails, domains, ip's and words by blocking user rregistrations, comments, messages, contacts, feedbacks or threads.
- [Webform](https://www.drupal.org/project/webform) - Webform is the module for making forms and surveys in Drupal.
  - [Webform videos on Drupal.org](https://www.drupal.org/docs/8/modules/webform/webform-videos) - A series of videos by the makers of Webform explaining features and tutorials for installing and using the Webform module.

### Media
- [Blazy](https://www.drupal.org/project/blazy) - Provides integration with bLazy to lazy load and multi-serve images to save bandwidth and server requests. The user will have faster load times and save data usage if they don't browse the whole page.
- [Image Optimize (or ImageAPI Optimize)](https://www.drupal.org/project/imageapi_optimize) - This is a toolkit for ImageAPI. It requires imageapi_gd or imageapi_imagemagick or any ImageAPI toolkit to work.
- [Media](https://www.drupal.org/project/media) - The Media module provides an extensible framework for managing files and multimedia assets, regardless of whether they are hosted on your own site or a 3rd party site - it is commonly referred to as a 'file browser to the internet'.
- [PhotoSwipe](https://www.drupal.org/project/photoswipe) - Use PhotoSwipe to display picture galleries on your Drupal website. This Javascript lightbox library offers very nice mobile browsing features (in particular swiping to the next picture)!
  - Note: As for the `1.0-beta3` release, it needs to be [patched](https://www.drupal.org/files/issues/path-capitals-for-composer-2855483-2.patch) when installed with Composer.
- [Slick Carousel](https://www.drupal.org/project/slick) - Slick is a powerful and performant slideshow/carousel solution leveraging Ken Wheeler's Slick carousel.
  - Also make sure to check out it's sub modules such as e.g. [Slick Paragraphs](https://www.drupal.org/project/slick_paragraphs) or [Slick Entity Reference](https://www.drupal.org/project/slick_entityreference).
- [Video](https://www.drupal.org/project/video) - Video module allows you to upload video in any format, play video in any format, transcode video to H.246, Theora, VP8(Web compatible formats) using Zencoder or FFMPEG automatically creates video thumbnails, copy and deliver videos from cloud file systems like Amazon S3.
- [Video Embed Field](https://www.drupal.org/project/video_embed_field) - Video Embed field creates a simple field type that allows you to embed videos from YouTube and Vimeo and show their thumbnail previews simply by entering the video's url.

### Migration
- [Migrate Plus](https://www.drupal.org/project/migrate_plus) - The migrate_plus project provides extensions to core migration framework functionality, as well as examples.
- [Migrate Source CSV](https://www.drupal.org/project/migrate_source_csv) - This project allows you to import CSV files using Drupal Migration.
- [Migrate Tools](https://www.drupal.org/project/migrate_tools) - The Migrate Tools module provides tools for running and managing Drupal 8 migrations.

### Multilingualism
- [Language Cookie](https://www.drupal.org/project/language_cookie) - Adds an extra "Cookie" field to the Language Negotiation settings, allowing the language to be set according to a cookie.

### Multisite
- [Domain Access](https://www.drupal.org/project/domain) - The Domain Access project is a suite of modules that provide tools for running a group of affiliated sites from one Drupal installation and a single shared database.

### Performance
- [Advanced CSS/JS Aggregation](https://www.drupal.org/project/advagg) - AdvAgg allows you to improve the frontend performance of your site.
- [CDN](https://www.drupal.org/project/cdn) - This module provides easy Content Delivery Network integration for Drupal sites. It changes file URLs, so that files (CSS, JS, images, fonts, videos …) are downloaded from a CDN instead of your web server.
- [DB Maintenance](https://www.drupal.org/project/db_maintenance) - DB maintenance optimizes administrator-selected tables in the database during regular cron.php executions.
- [Memcache API and Integration](https://www.drupal.org/project/memcache) - This module provides integration between Drupal and Memcached.

### Search
- [Custom Search](https://www.drupal.org/project/custom_search) - This module alters the default search box in many ways. If you need to have options available like in advanced search, but directly in the search box, this module is for you.
- [Elasticsearch Connector](https://www.drupal.org/project/elasticsearch_connector) - Elasticsearch Connector is a set of modules designed to build a full Elasticsearch eco system in Drupal.
- [Search API](https://www.drupal.org/project/search_api) - This module provides a framework for easily creating searches on any entity known to Drupal, using any kind of search engine.
- [Search API Solr Search](https://www.drupal.org/project/search_api_solr) - This module provides a Solr backend for the Search API module.
- [Search Autocomplete](https://www.drupal.org/project/search_autocomplete) - This module allows you to add autocomplete functionality to virtually any fields of a Drupal site. During the input, the field will be expanded and offers a list of suggestions before you start the search.

### Security
- [Automatic Updates](https://www.drupal.org/project/automatic_updates) - A project for organizing the Auto Updates Initiative efforts, as proposed in this idea.
- [Password Reset Landing Page (PRLP)](https://www.drupal.org/project/prlp) - The Password Reset Landing Page "PRLP" module enhances the original password reset landing page by letting a user set their new password at the same time they "log in" using the one-time-login link.
- [Password Strength](https://www.drupal.org/project/password_strength) - The Password Strength module provides realistic password strength measurement and server-side enforcement for Drupal sites using pattern-matching and entropy calculation.
- [Persistent Login](https://www.drupal.org/project/persistent_login) - The Persistent Login module provides a "Remember Me" option on the user login form.
- [Protected Pages](https://www.drupal.org/project/protected_pages) - Protected Pages modules allows the administrator to secure any page in your website by password.
- [Rabbit Hole](https://www.drupal.org/project/rabbit_hole) - Rabbit Hole is a module that adds the ability to control what should happen when an entity is being viewed at its own page.
- [Security Kit](https://www.drupal.org/project/seckit) - SecKit provides Drupal with various security-hardening options.
- [Shield](https://www.drupal.org/project/shield) - PHP Authentication shield. It creates a simple shield for the site with Apache authentication.

### SEO / Analytics
- [Google Analytics](https://www.drupal.org/project/google_analytics) - Adds the Google Analytics web statistics tracking system to your website.
- [Metatag](https://www.drupal.org/project/metatag) - The Metatag module allows you to automatically provide structured metadata, aka "meta tags", about a website.
- [Pathauto](https://www.drupal.org/project/pathauto) - The Pathauto module automatically generates URL/path aliases for various kinds of content (nodes, taxonomy terms, users) without requiring the user to manually specify the path alias.
- [Piwik Web Analytics](https://www.drupal.org/project/piwik) - Adds the Piwik web statistics tracking system to your website.
- [Redirect](https://www.drupal.org/project/redirect) - Manage custom site redirects.
- [SEO Checklist](https://www.drupal.org/project/seo_checklist) - The Drupal SEO Checklist uses best practices to check your website for proper search engine optimization. It eliminates guesswork by creating a functional to-do list of modules and tasks that remain.
- [Simple XML sitemap](https://www.drupal.org/project/simple_sitemap) - Every webpage needs an automatic XML sitemap generator for SEO reasons. This module aims to be a replacement for the xmlsitemap module for Drupal 8.

### Site building
- [@font-your-face](https://www.drupal.org/project/fontyourface) - @font-your-face provides an administrative interface for browsing and applying web fonts (using CSS @font-face, supported in all popular browsers) from a variety of sources.
- [Admin Toolbar](https://www.drupal.org/project/admin_toolbar) - The Admin Toolbar intends to improve the default Drupal Toolbar (the administration menu at the top of your site) to transform it into a drop-down menu, providing a fast access to all administration pages.
- [Block Group](https://www.drupal.org/project/blockgroup) - This module extends the standard Drupal block system with block groups. Each block group provides a new block as well as a corresponding region. Child blocks can be moved into any group region.
- [Block Visibility Groups](https://www.drupal.org/project/block_visibility_groups) - Block Visibility Groups allows the site administrator to easily manage complex visibility settings that apply to any block placed in a visibility group.
- [Easy Breadcrumb](https://www.drupal.org/project/easy_breadcrumb) - The Easy Breadcrumb module provides a plug-and-play block to be embedded in your pages, typically at some place near the page's header.
- [Entity Browser](https://www.drupal.org/project/entity_browser) - The goal of this module is to provide a generic entity browser/picker/selector.
- [Field Group](https://www.drupal.org/project/field_group) - Fieldgroup will, as the name implies, group fields together. All fieldable entities will have the possibility to add groups to wrap their fields together.
- [GraphQL](https://www.drupal.org/project/graphql) - This module lets you craft and expose a GraphQL schema for Drupal 8.
- [Linkit - Enriched linking experience](https://www.drupal.org/project/linkit) - Linkit provides an easy interface for internal and external linking with wysiwyg editors by using an autocomplete field.
- [Menu Breadcrumb](https://www.drupal.org/project/menu_breadcrumb) - This module allows you to use the menu the current page belongs to for the breadcrumb, generating breadcrumbs from the titles of parent menus.
- [Menu Item Extras](https://www.drupal.org/project/menu_item_extras) - Menu Item Extras provides extra fields for menu items without using additional entities.
- [Menu Link Attributes](https://www.drupal.org/project/menu_link_attributes) - This module allows you to add attributes to your menu links.
- [Menu Link Weight](https://www.drupal.org/project/menu_link_weight) - This module replaces the standard numeric weight dropdown widget for menu links in the node form with a tabledrag widget that lists all children for the selected parent.
- [Menu Trail By Path](https://www.drupal.org/project/menu_trail_by_path) - Menu Trail By Path sets the active-trail on menu items according to the current url.
- [Paragraphs](https://www.drupal.org/project/paragraphs) - Paragraphs is the new way of content creation! It allows you — Site Builders — to make things cleaner so that you can give more editing power to your end-users.
  - Also check out [Paragraphs Edit](https://www.drupal.org/project/paragraphs_edit)
  - .. and this [blog post](https://www.ostraining.com/blog/drupal/paragraphs-module/)
- [Reroute Email](https://www.drupal.org/project/reroute_email) - This module intercepts all outgoing emails from a Drupal site and reroutes them to a predefined configurable email address.
- [Simple hierarchical select](https://www.drupal.org/project/shs) - Simple hierarchical select defines a new form widget for taxonomy fields to select a term by "browsing" through the vocabularies hierarchy.
- [Token](https://www.drupal.org/project/token) - Provides additional tokens not supported by core (most notably fields), as well as a UI for browsing tokens.
- [Vertical Tabs Config](https://www.drupal.org/project/vertical_tabs_config) - This module allows you to hide and re-order vertical tabs on add/edit node pages depending on content type and role.

### Site navigation
- [Responsive and off-canvas menu](https://www.drupal.org/project/responsive_menu) - This module integrates the mmenu jQuery plugin with Drupal's menu system with the aim of having an off-canvas mobile menu and a horizontal menu at wider widths.

### Social media
- [AddToAny Share Buttons](https://www.drupal.org/project/addtoany) - Share buttons for Drupal including the AddToAny universal share button, Facebook, Twitter, Google+, Pinterest, WhatsApp and many more.
- [Ridiculously Responsive Social Sharing Buttons](https://www.drupal.org/project/rrssb) - Social sharing buttons that you can drop into any website with attractive SVG-based icons, small download, and browser compatibility. No 3rd-party scripts.

### User & Roles management
- [Auth0 Single Sign On](https://www.drupal.org/project/auth0) - Single Sign On for Enterprises + Social Login + User/Passwords. For all your Drupal instances. Powered by Auth0.
- [Email Registration](https://www.drupal.org/project/email_registration) - Allow users to register and login using only an email address. Users can then log-in using their email address and password for authentication.
- [Group](https://www.drupal.org/project/group) - The Group module allows you to create arbitrary collections of your content and users on your site and grant access control permissions on those collections.
- [Permissions by Term](https://www.drupal.org/project/permissions_by_term) - The Permissions by Term module extends Drupal by functionality for restricting access to single nodes via taxonomy terms.
- [RoleAssign](https://www.drupal.org/project/roleassign) - RoleAssign specifically allows site administrators to further delegate the task of managing user's roles while withholding the Administer permissions permission.
- [Taxonomy access fix](https://www.drupal.org/project/taxonomy_access_fix) - This module adds more specific Taxonomy permissions.

### Views
- [Better Exposed Filters](https://www.drupal.org/project/better_exposed_filters) - The Better Exposed Filters module replaces the Views' default single- or multi-select boxes with radio buttons or checkboxes, respectively.
- [DraggableViews](https://www.drupal.org/project/draggableviews) - DraggableViews makes rows of a view "draggable" which means that they can be rearranged by Drag'n'Drop.
- [Views Conditional](https://www.drupal.org/project/views_conditional) - Views Conditional is a simple module that allows you to define conditionals (if xxx then yyy) with fields in views.
- [Views Infinite Scroll](https://www.drupal.org/project/views_infinite_scroll) - Views infinite scroll allows you to load and display pages of any view inline, using AJAX (this has been called infinite scrolling, load more, autopaging, endless pages and more).
- [Views Reference Field](https://www.drupal.org/project/viewsreference) - This field in conjunction with the Paragraphs module, makes for a very powerful content management system, allowing addition of just about any kind of content into an entity page.

## Themes

### Frontend themes
- [AdaptiveTheme](https://www.drupal.org/project/adaptivetheme) - Adaptivetheme for Drupal 8 is a base theme designed for people who don’t code, or for those who only want to write a bit of CSS but still want a sleek and sophisticated theme for todays mobile web - and beyond.
- [Bootstrap](https://www.drupal.org/project/bootstrap) - This base theme bridges the gap between Drupal and the Bootstrap Framework.
- [Drupal8 Zymphonies Theme](https://www.drupal.org/project/drupal8_zymphonies_theme) - Drupal8 Zymphonies Theme is the first Zymphonies Drupal 8 Free Responsive Theme which has many new features.
- [ZURB Foundation](https://www.drupal.org/project/zurb_foundation) - Zurb Foundation for Drupal is the official implementation of the framework by the same name.

### Admin themes
- [Adminimal - Responsive Administration Theme](https://www.drupal.org/project/adminimal_theme) - A modern and minimalist design that makes administration an easy and fun experience.
  - Also install [Adminimal Admin Toolbar](https://www.drupal.org/project/adminimal_admin_toolbar) when using this theme.

## Troubleshooting
Every software has bugs. At least if it does more than simply printing out a `Hello World`.
While we're not able to write bugless software, we can still try to handle bugfixing as smooth as possible.  
So, what do you do when you find a bug in a module, theme or maybe even Drupal core?
Or if you simply just need a little help? Let's try figuring this out in the next sections.

### Update to the latest stable release
This step is extremely obvious, but maybe there has been a newer **stable** release of the module since your installation.  
Check if you have the newest stable version of the project, the bug might have been fixed in the meantime.

### Read the project's description
The second step might be obvious too but I still want to point it out. Everyone is free to contribute to Drupal and while
most Drupal-related things happen on Drupal.org itself, there are a few exceptions. So read the project's description
carefully! [Drupal console](https://www.drupal.org/project/console) e.g. chose to handle bug reports/feature requests
on GitHub. [Drupal commerce](https://www.drupal.org/project/commerce) offers contribution support on [IRC](#get-in-touch-with-the-drupal-community).

### Issue queue
Drupal projects normally work with *issue queues* (if nothing else defined), meaning that every project (Drupal core/module/theme/distribution/etc.) has it's
own issue queue. An issue can be everything from a bug report, task, feature request, support request, or just a plan.  
You can read more about issue queues on [drupal.org](https://www.drupal.org/issue-queue).  

So, if you've found a bug in a project, there's a high chance that the bug was already reported or maybe even fixed.
On a project's page, search for `All issues` and click on the `x open` (x = number of open issues) link.  
This link will take you to the project's issue queue.  

**Important:** Drupal core is a Drupal project itself. It has it's own issue queue and release pages.  
See the Drupal core project's page on [Drupal.org](https://www.drupal.org/project/drupal).

#### Finding your issue in the queue
In the issue queue the first thing you want to do, is filtering the issues by a major version.  
If the module has been around since Drupal 6/7/maybe even longer, you're less interested in the legacy issues.  
So change the **Version** filter to e.g. `- 8.x issues -`.

If you still didn't find your issue, try changing the **Status** from `- Open issues -` to `- Any -`.  
It's possible that the issue has already been fixed but not released yet.

#### Creating an issue
If you didn't find your issue, you can create a new one. Make sure to be **as precise and specific as possible**.  
Include the exact version of Drupal and the exact module/theme/distribution version.
Write how to reproduce the bug on a **fresh Drupal installation**. Speaking about, you might want to check if the
bug also occurs on a fresh Drupal installation with only the needed modules/themes installed.  
Maybe it's a bug that only occurs when certain other modules/themes are installed?  

Keep in mind that many projects are being contributed by developers in their free time. A project maintainer
might respond very quickly to a new issue but sometimes it can take weeks or even months until you get a reply.
In the meantime, you can try to get in touch with other Drupal developers who might be able to help you out.
Check the next sections for more information.

### Drupal Answers
As a developer, you probably came around Stack Overflow when trying to fix an issue.  
**Good news:** There's a Stack Exchange for Drupal as well! It's called **Drupal Answers**, [have a look](https://drupal.stackexchange.com/).

### Google
If you were unlucky finding answers via the issue queue/Drupal Answers, maybe someone wrote a blog post or a tutorial
which could help you in solving your issue.  
Now before you go on something like "But Googling is obvious", let me give you **one important tip**:

- Limit your search results to a specific time frame!

If you search for a commerce issue for example, the probability is high to find solutions to the Drupal 7 version of it.
But if you're interested in a solution for the Drupal 8+ versions, you're better off limiting the search results by e.g.
publish date and only show results from the past year on.  
The date limitation is only one thing you can do, there are a lot of articles on how to google efficiently out there, read them!

### IRC / Slack support
If you still weren't able to find a solution to your issue, you can write to other Drupal developers via IRC or Slack.  
Check the [Get in touch with the Drupal community](#get-in-touch-with-the-drupal-community) section on how to connect to them.

When asking for help, keep in mind that it's not self-evident to help many other people in complicated matters.
Be friendly, try describing your issue as precisely as possible and maybe a good fellow will help you out.

## Contributing to Drupal
Are you happy with Drupal and would you like to give back? That's **great**!
There are many different way on how to contribute back. You can improve documentation, add translations, create
new contrib projects or simply donate.  
Please follow the *Ways to Get Involved* guide on [Drupal.org](https://www.drupal.org/contribute).

One important tip though: Starting to contribute *can* be a little bit tough and difficult in the beginning.
If you have the chance to visit A Drupal camp or conference or maybe even just a meetup, try to get some guided help there.
Some things are a little bit complicated but every experienced Drupal developer will most-likely try in helping you out.  
**Don't** be afraid to ask for help! I quote from Drupal:
> Come for the Code, Stay for the Community.

## Video tutorial
Find below a few video resources that are really worth your time.  
**Important:** There's also [Drupal.tv](https://drupal.tv/), check it out!

### Beginner training series
- [Drupal 8 Beginner Tutorials](https://www.youtube.com/playlist?list=PLtaXuX0nEZk9MKY_ClWcPkGtOEGyLTyCO) - A 63 video training course by OSTraining introducing the basics of Drupal 8. Designed for absolute beginners, it assumes no prior experience with Drupal and does a great job of explaining the basics.
- [Build Your First Drupal 8 Site in 1 Hour](https://www.youtube.com/playlist?list=PLtaXuX0nEZk-Mer_a_P1sp0mroJGVs6TK) - An 11 video course by OSTraining that goes over "how to create content, use Views, add contact forms and choose themes".
- [How To Install Drupal 8 Sites](https://www.youtube.com/playlist?list=PLtaXuX0nEZk99zgSc19Li8EsM9jkicDQj) - A 5 video course by OSTraining going over the basics on how to download, install and set up a Drupal 8 site.
- [How to Update Drupal 8 Sites, Modules, Themes](https://www.youtube.com/playlist?list=PLtaXuX0nEZk-_lYMB0ehySQEfssaCU1jZ) - A 5 video course by OSTraining explaining how to update Drupal 8 sites, modules and themes.
- [How to Backup and Restore Drupal 8 Sites](https://www.youtube.com/playlist?list=PLtaXuX0nEZk_y_xlcAv_Ub_xLCfvF8TSs) - A 5 video course by OSTraining explaining how to backup the files and database for a site as well as restore them.

### General
- [Rendering & caching: a journey through the layers](https://www.youtube.com/watch?v=MQGUzubY35I) - Understand the basics of the Render and Cache API.

### Modules
- Webform
  - [Videos on Drupal.org](https://www.drupal.org/docs/8/modules/webform/webform-videos) - A series of videos by the makers of Webform explaining features and tutorials for installing and using the Webform module.

### Theming
- [Decouple your Twig from PHP and make Frontenders happy!](https://www.youtube.com/watch?v=Z4gMLSD5MAU) - A talk about using Drupal + Fractal + Node.js.
- [Building your first Drupal 8 Theme](https://www.youtube.com/watch?v=5GxsmuWFV3M) - A guide helping you to create your first Drupal theme step by step.

## Blog posts
- [Drupal 8: Hooks, Events, and Event Subscribers](https://www.daggerhart.com/drupal-8-hooks-events-event-subscribers/)
- [Set Required and Optional Address Inputs for Address Field in Drupal 8](https://timonweb.com/posts/set-required-and-optional-address-inputs-for-address-field-in-drupal-8/)
- [How to Change the Default Text Strings in Drupal 8](https://www.ostraining.com/blog/drupal/translate-drupal-8-strings/)
- [Stop Waiting for Feeds Module: How to Import RSS in Drupal 8](https://ohthehugemanatee.org/blog/2017/06/07/stop-waiting-for-feeds-module-how-to-import-remote-feeds-in-drupal-8/)
- [Using Responsive Images in Drupal 8](https://www.bluecoda.com/blog/using-responsive-images-drupal-8)
- [Set up workflows with State machine on Drupal 8](https://www.flocondetoile.fr/blog/set-workflows-state-machine-drupal-8)
- [Converting a non-Composer Drupal codebase to use Composer](https://www.jeffgeerling.com/blog/2018/converting-non-composer-drupal-codebase-use-composer)
- [Drupal 8 Add Cache Metadata to Render Arrays](https://weknowinc.com/blog/drupal-8-add-cache-metadata-render-arrays)
- [Integrate Webform and Google Sheets using Zapier in Drupal 8](https://www.webwash.net/integrate-webform-and-google-sheets-using-zapier-in-drupal-8/)
- [How to Set a Voting System in Drupal 8](https://www.ostraining.com/blog/drupal/voting-system/)
- [The Ultimate Tutorial for Drupal's Paragraphs Module](https://www.ostraining.com/blog/drupal/paragraphs-module/)
- [Drupal 8’s mail sending opportunities](https://internetdevels.com/blog/mail-sending-drupal-8)
- [Top 2018 Drupal Modules using Artificial Intelligence](https://opensenselabs.com/blog/tech/top-2018-drupal-modules-using-artificial-intelligence)
- [Using partial Twig templates](https://befused.com/drupal/partial-twig)
- [Visual Regression Testing with BackstopJS](https://www.davidneedham.me/drupaleu2018/)
- [Composer Best Practices for Updating Drupal 8 Core and Modules](https://www.grazitti.com/blog/why-composer-is-the-best-practices-for-updating-drupal-8-core-and-modules/)
- [Testing the 'Add user' and 'Edit account' forms in Drupal 8 with Behat](https://www.jeffgeerling.com/blog/2018/testing-add-user-and-edit-account-forms-drupal-8-behat)
- [Simple Guzzle API mocking for functional testing in Drupal 8](https://www.webomelette.com/simple-guzzle-api-mocking-functional-testing-drupal-8)
- [Decoupled Drupal Authentication with JSON Web Tokens](https://dev.acquia.com/blog/decoupled-drupal-authentication-json-web-tokens)
- [Automatic removal of .git directories from Composer dependencies](https://www.drupaleasy.com/quicktips/automatic-removal-git-directories-composer-dependencies)
- [Make composer operations with Drupal way faster and easier on RAM](https://www.jeffgeerling.com/blog/2018/make-composer-operations-drupal-way-faster-and-easier-on-ram)
- [How to Create a Node in Drupal 8 using REST](https://www.agiledrop.com/blog/how-create-node-drupal-8-using-rest)
- [Provide a custom mode form to entities with Drupal 8](https://www.flocondetoile.fr/blog/provide-custom-mode-form-entities-drupal-8)
- [Drupal 8 Configuration Management with Config Split](https://www.daggerhart.com/drupal-8-configuration-management-with-config-split/)
- [Writing Automated Tests in Drupal 8, Part 1: Test types and set up](https://deninet.com/blog/2018/12/31/writing-automated-tests-drupal-8-part-1-test-types-and-set)
- [Writing Automated Tests in Drupal 8, Part 2: Functional tests](https://deninet.com/blog/2019/01/13/writing-automated-tests-drupal-8-part-2-functional-tests)
- [Writing Automated Tests in Drupal 8, Part 3: Unit tests](https://deninet.com/blog/2019/01/27/writing-automated-tests-drupal-8-part-3-unit-tests)
- [Keeping your Drupal 8 modules, themes and custom code continually up to date, preparing for Drupal 9](http://hojtsy.hu/blog/2019-feb-06/keeping-your-drupal-8-modules-themes-and-custom-code-continually-date-preparing)
- [How to Create a Product Catalog with Search API, Solr and Facets](https://blog.acromedia.com/how-to-create-a-product-catalog-with-search-api-solr-and-facets)
- [Reuse readme.md in hook_help() with Parsedown](https://colorfield.be/blog/reuse-readmemd-hookhelp-parsedown)
- [Controlling multiple sites with Drush 9](http://www.noreiko.com/blog/controlling-multiple-sites-drush-9)
- [Doping for editors: Put the fun in Paragraphs](https://www.undpaul.de/en/blog/2019/04/12/doping-editors-put-fun-in-paragraphs)
- [Recognizing Insecure Drupal Code](https://thinkshout.com/blog/2019/05/recognizing-insecure-drupal-code)
- [Using Config Split and Config Ignore to Fine-Tune Your Configuration Management Process](https://www.o8.agency/blog/tips-dev-team-using-config-split-and-config-ignore-fine-tune-your-configuration-management)
- [Migrate from a CSV to Content Entities with Paragraphs](https://colorfield.be/blog/migrate-csv-to-content-entities-with-paragraphs)
- [Migrating files and images into Drupal](https://agaric.coop/blog/migrating-files-and-images-drupal)
- [Migrating data into Drupal subfields](https://agaric.coop/blog/migrating-data-drupal-subfields)
- [Invalidate the page cache according to a duration with Drupal 8](https://www.flocondetoile.fr/blog/invalidate-page-cache-according-duration-drupal-8)
- [Customise scaffold files the right way](https://www.computerminds.co.uk/articles/customise-scaffold-files-right-way)
- [Automatically remove the Drupal core README (and other) scaffolding files](https://www.drupaleasy.com/quicktips/automatically-remove-drupal-core-readme-and-other-scaffolding-files)
- [Customizing a CSV export with Entity Export CSV on Drupal 8](https://www.flocondetoile.fr/blog/customizing-csv-export-entity-export-csv-drupal-8)
- [How to Test Your Drupal Site's Accessibility](https://evolvingweb.ca/blog/how-test-your-drupal-sites-accessibility)
- [Drupal 8 content migrations from CSV or spreadsheet](https://atendesigngroup.com/articles/drupal-8-content-migrations-csv-spreadsheet)
- [How To Add Filter Effects to Images on your website with Image effects module](https://drudesk.com/blog/image-effects-module-for-drupal-8)
- [How to Import External Feeds into your Drupal 9 Website with the Feeds Module](https://www.specbee.com/blogs/how-import-external-feeds-your-drupal-9-website-feeds-module)

## Further resources
- [Comparison of Node/Entity Ordering Modules](https://www.drupal.org/node/398508)
- [Drupal Pitch Deck](https://www.drupal.org/community/agency-marketing/pitch-deck)

## Drupal PaaS
When it comes to hosting a Drupal site, you can always use any server which supports the system requirements.
However, there are a few Drupal specialized PaaS hosting options you might want to consider as well.

- [Acquia Cloud](https://cloud.acquia.com/)
- [amazee.io](https://www.amazee.io/)
- [Pantheon](https://pantheon.io/)
- [Platform.sh](https://platform.sh/)

## Get in touch with the Drupal community
If you wish to get more involved with the Drupal community, or want to get in contact with Drupal developers, you can use one of the following platforms.
- [DrupalChat](https://drupalchat.eu/) - An open source ([Rocket.Chat](https://rocket.chat/)) alternative to Slack.
- [Drupical](https://www.drupical.com/) - Find Drupal events with ease in a map! Note: The list is not complete but can give you a rough overview of Drupal events around the world.
- [IRC](https://www.drupal.org/ircchat) - Chat with the Drupal Community on IRC!
- [Meetups](https://www.meetup.com/topics/drupal/) - Participate in local Drupal meetups in your area and meet the community face to face.
- [Reddit](https://www.reddit.com/r/drupal/) - The Drupal community on Reddit. They have weekly rotating posts!
- [Slack](https://www.drupal.org/slack) - A list of Drupal Slack spaces and channels.
- [Twitter](https://twitter.com/) - Yes, a lot of us are on Twitter too! `#drupal`

## Drupal newsletter
Get the best Drupal news, tutorials and articles once a week without hours of browsing.  
Check out the [TheWeeklyDrop](http://www.theweeklydrop.com/).

## Credits
- [David Pacassi Torrico](https://www.drupal.org/u/dpacassi) - Project maintainer

## License
```
MIT License

Copyright (c) 2018 David Pacassi Torrico

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
