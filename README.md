# Steps to reproduce

1. Pull this repository
2. Run `npm i`
3. Run `npm run locales:update:ja`

See whether next error is showing up:
```shell
> ttag update --sortByMsgid true --addComments 'translator:' --extractLocation never "locales/ja.po" "src/"

⠋ [ttag] updating locales/ja.po ...Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-property-in-object since the "loose" mode option was set to "true" for @babel/plugin-proposal-class-properties.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-property-in-object", { "loose": true }]
to the "plugins" section of your Babel config.
Though the "loose" option was set to "false" in your @babel/preset-env config, it will not be used for @babel/plugin-proposal-private-methods since the "loose" mode option was set to "true" for @babel/plugin-proposal-private-property-in-object.
The "loose" option must be the same for @babel/plugin-proposal-class-properties, @babel/plugin-proposal-private-methods and @babel/plugin-proposal-private-property-in-object (when they are enabled): you can silence this warning by explicitly adding
	["@babel/plugin-proposal-private-methods", { "loose": true }]
to the "plugins" section of your Babel config.
✔ locales/ja.po updated
```