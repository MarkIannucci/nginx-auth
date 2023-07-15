# Fly.io Nginx basic auth example

Check this repo out. Run `fly launch` and say 'yes' to copy the config. Choose an app name. Choose not to deploy.

Now run `fly secrets set PASSWORD=somepassword`. Update the `proxy_pass` line in `nginx.conf` to the correct application name you wish to proxy requests to.

Finally, run `fly deploy`. You should be able to access your proxy app at `https://newappname.fly.dev`
