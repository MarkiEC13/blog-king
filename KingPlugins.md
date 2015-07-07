## Preface ##

Most of my plugins depend on some basic libraries inside the plugins/king-includes/ folder.
So if you just want to use some single plugins (wich is perfectly ok) you always need the king-includes Folder!
Some 3rd Partyplugins had to be adapted to fit into the enhanced plugins folderstructure. see next point.
My advice at this time is(for normal wordpress users), to pick out my plugins(which will work in the default pluginfolder) and get the 3rd party plugins from their maintainers location.

### Folder / Filestructure ###

You might be wondering why all plugins are nested in subfolders again: wp-content/plugins/king-admin/plugins/...
I wanted to keep my backend and the folders clean so i decided to do it this way. Another reason is, that you can easily disable a whole section and this way quickly test where a problem with a plugin occurs. The hookfile for this is inside the wp-admin folder named admin-king-plugins.php

If you also want to adapt this structure you MUST check that plugins, you put in there, have the right include/require pathes to other wordpress files set. The easiest way is to search inside those plugins for "/plugins/" or "../../"

You will find two changed corefiles which are wp-admin/index.php and admin-footer.php
Those are slightly cleaned(clean startpage/other footerlinks) and will be removed if i find the time to make a plugin for it.



## King Widgets ##

Those plugins only work with the widgets Plugin released by automattic or my jQueryfied version all of those can be found here in the repo:
http://blog-king.googlecode.com/svn/trunk/blog-king/wp-content/plugins/king-widgets/

[![](http://www.blog.mediaprojekte.de/wp-content/wp-filez/king_framework_wappen.jpg)](http://www.blog.mediaprojekte.de/cms-systeme/wordpress-plugins/king-widget-framework/) [![](http://www.blog.mediaprojekte.de/wp-content/wp-filez/king_categories_wappen.jpg)](http://www.blog.mediaprojekte.de/cms-systeme/wordpress/wordpress-widget-king-categories/) [![](http://www.blog.mediaprojekte.de/wp-content/wp-filez/king_pages_wappen.jpg)](http://www.blog.mediaprojekte.de/cms-systeme/wordpress-plugins/wordpress-widget-king-pages/) [![](http://www.blog.mediaprojekte.de/wp-content/wp-filez/king_links_wappen.jpg)](http://www.blog.mediaprojekte.de/cms-systeme/wordpress-plugins/wordpress-widget-king-links/) [![](http://www.blog.mediaprojekte.de/wp-content/wp-filez/king_rss_wappen.jpg)](http://www.blog.mediaprojekte.de/cms-systeme/wordpress-plugins/wordpress-widget-king-rss/)