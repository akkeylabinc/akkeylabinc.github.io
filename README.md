## Troubleshooting
> Installing eventmachine 1.2.7 with native extensions
> Gem::Ext::BuildError: ERROR: Failed to build gem native extension.
> ...
> An error occurred while installing eventmachine (1.2.7), and Bundler cannot continue

```sh
gem install eventmachine -v '1.2.7' -- --with-ldflags="-Wl,-undefined,dynamic_lookup"
```
https://github.com/eventmachine/eventmachine/issues/960

