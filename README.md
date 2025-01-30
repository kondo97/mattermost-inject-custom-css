# Mattermost Inject Custom CSS

This plugin allows you to inject custom CSS into Mattermost.

## Usage
Sorry, this plugin does not yet allow specifying CSS from the admin console.
Therefore, you need to build the plugin on your own.
1. Clone the repository.
2. Customize the CSS in `webapp/src/components/root_styles/styles.css`.
3. Run ``make``, then ``/dist/com.mattermost.inject-custom-css-XXX.tar.gz`` would be created.
4. Upload the plugin to your Mattermost server.

## Caution
This plugin uses registerRootComponent, so it will only work on the /team/XXX page. I believe this will cover almost all cases. Other pages, such as /login, will not be affected.
