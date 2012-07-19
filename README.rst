jQuery Translate
================

:Info: jQuery Translate is a translation plugin for jQuery. Is very useful in static html page.
:Author: Benoît Bar (http://github.com/benoitbar, http://www.scopart.fr/)

Instructions
============

Include the script in your page
    
    ...
    <script src="js/jquery.translate.min.js"></script>
    ...

Add a css class for all html tag content you want to translate
    
    ...
    <p class="trans">My text to translate</p>
    ...

Call the plugin with or without options

    $('.trans').translate({
        lang : 'en',
        url : '/local/',            // Determine the url where the translation file are
        showTranslations : false    // Show a strutured translation file in browser console
    });

or    

    $('.trans').translate();

Options
=======

*lang* (optional) : Determine the language to translate to. Set to browser language by default.

*url* (optional) : Determine the url where the translation files are. Set to /local/ by default. You must create one file by language naming them <language>.json. For example fr.json, en.json, ...

*showTranslations* : Show a strutured translation object in browser console. Set to false by default. You can set this parameter to true and then copy the object displayed in the browser console and paste it into your language json files.

Utils
=====

You can get browser language by calling i18n.getLang()

License
=======

jQuery Translate is Copyright © 2012 Benoît Bar. It is free software, and may be redistributed under the terms specified in the LICENSE file.