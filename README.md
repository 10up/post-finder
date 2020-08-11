# Post Finder

> Creates a rich input field that allows a user to curate and rank content items (posts or other custom post types)

[![Support Level](https://img.shields.io/badge/support-stable-blue.svg)](#support-level) [![Release Version](https://img.shields.io/github/release/10up/post-finder.svg)](https://github.com/10up/post-finder/releases/latest) ![WordPress tested up to version](https://img.shields.io/badge/WordPress-v5.4%20tested-success.svg) [![GPLv2 License](https://img.shields.io/github/license/10up/post-finder.svg)](https://github.com/10up/post-finder/blob/develop/LICENSE.md)


## Installation

Clone the plugin to your `wp-content/plugins/` directory.

## Usage

In your theme, you can call `pf_render( $name, $value, $options )` where you want to display a Post Finder field.

`$name` : Name you want to use on the input field

`$value` : Currently selected value(s). Should be a comma-separated string of post_ids

`$options` (optional) : Array of options that will be used to build the input

**Current options**
* `show_numbers` - Whether to show a positional number next to each item. Makes it easy to see which position each item has. Default true.
* `show_recent` - Whether to show the Recent Post select input. Default true.
* `limit` - Limit how many items can be selected. Default 10.
* `args` - Array of arguments passed to our `WP_Query` instances. Allows customizations of these queries, like setting a specific post type. See the [WordPress Developer Reference](https://developer.wordpress.org/reference/classes/wp_query/#methods-and-properties) for supported arguments.
* `include_script` - Whether to include the init script for the input. Default true. If false, you'll have to include this yourself in order for it to work.
```
jQuery( document ).ready( function( $ ) {
	$( '.post-finder' ).postFinder();
} );
```

## Support Level

**Stable:** 10up is not planning to develop any new features for this, but will still respond to bug reports and security concerns. We welcome PRs, but any that include new features should be small and easy to integrate and should not include breaking changes. We otherwise intend to keep this tested up to the most recent version of WordPress.

## Changelog

A complete listing of all notable changes to Post Finder are documented in [CHANGELOG.md](https://github.com/10up/post-finder/blob/develop/CHANGELOG.md).

## Contributing

Please read [CODE_OF_CONDUCT.md](https://github.com/10up/post-finder/blob/develop/CODE_OF_CONDUCT.md) for details on our code of conduct, [CONTRIBUTING.md](https://github.com/10up/post-finder/blob/develop/CONTRIBUTING.md) for details on the process for submitting pull requests to us, and [CREDITS.md](https://github.com/10up/post-finder/blob/develop/CREDITS.md) for a listing of maintainers of, contributors to, and libraries used by Post Finder.

## Like what you see?

<a href="http://10up.com/contact/"><img src="https://10up.com/uploads/2016/10/10up-Github-Banner.png" width="850" alt="Work with us at 10up"></a>
