AuthPack
========


General
-------

AuthPack is a demonstration project for .NET authentication with Twitter, Facebook, Google, and LinkedIn.  It includes sample oAuth API calls for each service.


Installation
------------

Most of the files in this solution are generated by the standard Visual Studio Web Forms template.

- Important: Update Web.config with service provider authentication keys and secrets.

- Site.Master - Contains most HTML/Javascript modifications.

- /Auth - Most of the custom code resides here. Auth.aspx.cs contains sample oAuth calls for each provider.

If someone would like to beautify the display of the buttons, I'd love to see that too.


oAuth Setup
-----------

Register your application with the service providers and retrieve the necesseary API keys.  Then enter them in web.config.

Twitter - https://dev.twitter.com/apps/new

Facebook - http://developers.facebook.com/docs/guides/web/

Google - https://code.google.com/apis/console/

LinkedIn - https://www.linkedin.com/secure/developer


Tips
----

Twitter is the easiest service to configure and get running.  Make sure you enter an oAuth Callback Url, even if you will override it in the application.

Facebook, Google, and LinkedIn require you to enter the domain from which you'll be accessing the services.  http://localhost should work, but you may need to update your hosts file for Facebook.

LinkedIn requires SSL.  This cannot be done on the Visual Studio Development Web Server.  You will have to setup IIS with https and debug in IIS.

