Sure, here's a more detailed guide:

1. **Check Nginx Configuration:** Run the following command to check the syntax of your Nginx configuration files:
    
    ```bash
    sudo nginx -t
    ```
    
    This command will verify the syntax of your Nginx configuration files and report any errors. It's a good practice to do this before restarting Nginx to ensure that your changes won't cause any issues.
    
2. **Locate Nginx Configuration Files:** After running the above command, you'll get information about the location of your Nginx configuration files. Look for the path displayed in the output. For example:
    
    ```bash
    Configuration file /etc/nginx/nginx.conf test is successful
    ```
    
    This indicates that the main configuration file is located at `/etc/nginx/nginx.conf`.
    
3. **Navigate to Configuration Directory:** Change your current directory to the directory where additional Nginx configuration files are stored. By default, Nginx may include configurations from the `conf.d` directory. You can navigate to this directory using the following command:
    
    ```bash
    cd /etc/nginx/conf.d
    
    ```
    
    In this directory, you'll typically find additional configuration files that are included in the main Nginx configuration. These files are often used to configure specific sites or applications.
    
4. **Modify Configuration Files:** Within the `conf.d` directory, you'll find various configuration files. These files may correspond to different websites or applications hosted on your server. For example:
    
    - `ultraapi.conf`
    - `uat_sse.conf`
    - `uat_redde_fmg.conf`
    - `uat_redde_northgate.conf`
    - `uat_drivetech.conf`
    - `uat_test.conf`
    - `uat_lkq_ultraportal.conf`
    - `uat_ultraportal.conf`
    
    Open the configuration file corresponding to the site or application you want to modify. You can use a text editor like `nano` or `vi` to make changes to these files:
    
    ```bash
    sudo vi uat_ultraportal.conf
    
    ```
    
    Within the configuration file, you can make modifications to various settings, including the theme of the site or application. Look for relevant directives such as `theme` or `style` to customize the appearance according to your preferences.
    
    ```bash
    fastcgi_param TENANT "theme";
    ```
    
    This can be changed to `vanilla`, `tfs`, `indicate` and more.
    
5. **Save Changes and Restart Nginx:** After making the necessary modifications to the configuration files, save the changes and exit the text editor. Then, restart Nginx to apply the new configurations:
    
    ```bash
    sudo nginx -s reload
    ```
    
    This command will restart the Nginx service, allowing the changes to take effect. Make sure to test the functionality of your website or application to ensure that the modifications were successful.