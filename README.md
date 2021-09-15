# GitLab Runner service

This is an initscript-style service to start/stop **Gi**tLab **Ru**nners on macOS.

> TODO: documentation

## configuration example

giru looks for its configuration file named `giru.plist` in `XDG_CONFIG_HOME` first and then in its own folder.

```plist
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>runner</key>
	<dict>
		<key>config_dir</key>
		<string>/Users/user01/.local/etc/gitlab-runner</string>
		<key>binary</key>
		<string>/opt/homebrew/bin/gitlab-runner</string>
	</dict>
</dict>
</plist>
```

## License

[GPL-2.0-or-later](LICENSE)