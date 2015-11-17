# heartfulness-uk
How to create the wordpress site on local system.
1. Download and install wamp from http://www.wampserver.com/en/
2. Make sure that wamp is running on your local system by going to localhost/ on any of the browser. There can be some port issues which are generally resolved by uninstalling skype as it uses the same port.
3. Goto localhost/phpMyAdmin and create an empty database(e.g. heartfulnessuk_db) which wordpress can refer to at a later stage.
4. Create a folder called heartfulness-uk in the www directory of the wamp server.
5. Push the repository content into this folder on your local system.
6. Run importbuddy.php on your local server by using the url localhost/heartfulness-uk/importbuddy.php
7. Follow the steps to unzip the site backup and create the folder structure on your local system.
8. There can be some issues, workaround for few of those are mentioned below:
    a.  Issue: While trying to create a backup for the file the execution process might exceed time and fail
        Workaround: Go to the wamp icon in the taskbar,hoveron PHP and increase the max_execution_time in php.ini. Then go to
                    C:\wamp\apps\phpmyadmin3.4.10.1\libraries (change path according to your installation)
                    open config.default.php and change value for $cfg['ExecTimeLimit'] to 0:
                    $cfg['ExecTimeLimit'] = 0;
    b.  Issue: 


To be cont...
