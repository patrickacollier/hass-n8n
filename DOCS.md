# Configuration

In the configuration section, set the port if the default one is not good for you. Enable auth if you want and SSL to.
Even if unused, let the default variables set.

## Addon Configuration

Add-on configuration:

```yaml
timezone: Europe/Berlin
env_vars_list: []
cmd_line_args: ""
```

### Option: `env_vars_list` (required)

List of the n8n environment variables. You can add as many environment variables as you want to the list through the UI. The format is the following :

`WEBHOOK_URL: https://mywebhookurl.com` (the regular expression is `^[A-Z_0-9]+: .*$` )

All the available environment variables are available here : <https://docs.n8n.io/hosting/environment-variables/environment-variables/>

#### Installing external packages

In n8n you can add external node modules by setting the `NODE_FUNCTION_ALLOW_EXTERNAL` environment variable with the list of npm packages you need.

For example, to install the `lodash` and the `moment` packages, in the UI, set the `env_vars_list` variable to:

```txt
NODE_FUNCTION_ALLOW_EXTERNAL: lodash,moment
```

### Option: `cmd_line_args` (optional)

The command line to start n8n. If you want to use a custom command line, you can use this variable.

## How to use it?
Just start the addon and head to the addon's web UI.

## Useful ressources

### Documentation

<https://docs.n8n.io>
<https://docs.n8n.io/getting-started/tutorials.html>

### Community public workflows

<https://n8n.io/workflows>

### Available integrations

<https://n8n.io/integrations>

## Support

Got questions?

You can open an issue on Github and i'll try to answer it

repository: <https://github.com/Rbillon59/hass-n8n>

## License

This addon is published under the apache 2 license. Original author of the addon's bundled software is n8n
