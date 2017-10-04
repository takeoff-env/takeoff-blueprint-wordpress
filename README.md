# Takeoff Wordpress Blueprint

This is a [Wordpress](https://github.com/WordPress/WordPress) blueprint provided for [Takeoff](https://github.com/takeoff-env/takeoff).

To install this blueprint, once you have Takeoff type:

```bash
npm run takeoff:new -- --env=wordpress --blueprintName=wordpress --submodule
```

This will create a Wordpress environment.  Using docker volumes, the source files are available in `env/wordpress`.

## Running Wordpress

Once the environment is created type

```bash
npm start -- --env=wordpress
```

This will start the app on port 80, so you can go to `[http://localhost/wp-admin/setup-config.php](http://localhost/wp-admin/setup-config.php)` to set up your site.  For Database Name, Username, Password enter `wp`.  For Database Host enter **`db`**.  You may then be asked to create a config file.  In your `env/wordpress` folder create a `wp-config.php` file and paste in the contents.

Then continue with the install.  It is recommended you have your own repository set up for the wordpress content and any database backups.
