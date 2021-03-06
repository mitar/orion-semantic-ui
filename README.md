# Semantic-UI Orion Admin Theme

This is the unstyled version of the Orion Admin Theme. This theme is a replica of the ```orionjs:bootstrap``` package. The markup and styles have been updated to use Semantic-UI. This package is for orion developers that would prefer to use semantic-ui for their projects.

> The current version is now stable with the latest orion version. Most style issues have been resolved. There is an issue with tabular since it uses bootstrap by default. I'm looking into updating tabular to use semantic-ui. Just bear with it for now.

## Demo

Demo for testing orion semantic ui admin theme. Please note, all data is published to the client, you would need to add more refined publications and subscriptions for production.

[DEMO](http://orion-semantic-ui.meteor.com)

> Login with username: admin // password: admin

## Installation

While in your meteor app's root, run the following from the command line:

```
$ meteor add dvz:orion-semantic-ui
```

## Package Details

This package depends on ```semantic:ui``` meteor package, so make sure you add it into your project. It will automatically add ```useraccounts:semantic-ui ```. Since Summernote relies on bootstrap, you would need to use ```orionjs:froala``` or another editor.

Additionally, this package makes use of ```fabienb4:autoform-semantic-ui``` so that autoform uses semantic-ui templates. However, you have to configure this on the client side, like so:

```
Meteor.startup(function() {
  AutoForm.setDefaultTemplate('semanticUI');
});
```
