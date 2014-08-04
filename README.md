# Semantic MediaWiki

[![Build Status](https://secure.travis-ci.org/SemanticMediaWiki/SemanticMediaWiki.svg?branch=master)](http://travis-ci.org/SemanticMediaWiki/SemanticMediaWiki)
[![Code Coverage](https://scrutinizer-ci.com/g/SemanticMediaWiki/SemanticMediaWiki/badges/coverage.png?s=f3501ede0bcc98824aa51501eb3647ecf71218c0)](https://scrutinizer-ci.com/g/SemanticMediaWiki/SemanticMediaWiki/)
[![Scrutinizer Quality Score](https://scrutinizer-ci.com/g/SemanticMediaWiki/SemanticMediaWiki/badges/quality-score.png?s=d9aac7e68e6554f95b0a89608cbc36985429d819)](https://scrutinizer-ci.com/g/SemanticMediaWiki/SemanticMediaWiki/)
[![Latest Stable Version](https://poser.pugx.org/mediawiki/semantic-media-wiki/version.png)](https://packagist.org/packages/mediawiki/semantic-media-wiki)
[![Packagist download count](https://poser.pugx.org/mediawiki/semantic-media-wiki/d/total.png)](https://packagist.org/packages/mediawiki/semantic-media-wiki)
[![Dependency Status](https://www.versioneye.com/php/mediawiki:semantic-media-wiki/badge.png)](https://www.versioneye.com/php/mediawiki:semantic-media-wiki)

Semantic MediaWiki (a.k.a. SMW) is a free, open-source extension to [MediaWiki]
(https://semantic-mediawiki.org/wiki/MediaWiki) – the wiki software that
powers Wikipedia – that lets you store and query data within the wiki's pages.

Semantic MediaWiki is also a full-fledged framework, in conjunction with
many spinoff extensions, that can turn a wiki into a powerful and flexible
knowledge management system. All data created within SMW can easily be
published via the [Semantic Web](https://semantic-mediawiki.org/wiki/Semantic_Web),
allowing other systems to use this data seamlessly.

For details and further links, see [the SMW wiki](https://semantic-mediawiki.org).

## Requirements

- PHP 5.3.2 or later
- MediaWiki 1.19 or later
- MySQL 5+ or SQLite 3+

A list of supported PHP versions, MediaWiki versions and databases per SMW release can be found
in the [compatibility matrix](COMPATIBILITY.md).

## Installation

The easiest way to install Semantic MediaWiki is by using [Composer][composer].
It is recommended to read the [installation instructions](docs/INSTALL.md) together with
the available [upgrade guide][smw-installation].

```json
{
	"require": {
		"mediawiki/semantic-media-wiki": "~2.0"
	}
}
```

## Documentation

Most of the documentation can be found on the [SMW wiki](https://semantic-mediawiki.org).
A small core of documentation also comes bundled with the software itself. This documentation
is minimalistic and less explanatory then what can be found on the SMW wiki. It is however
always kept up to date, and applies to the version of the code it comes bundled with.
The most important files are linked below.

* [User documentation overview](docs/README.md)
* [Developer documentation overview](docs/technical/README.md)


## Contribution and support

[![Twitter](https://semantic-mediawiki.org/w/images/c/c9/Twitter_icon.jpg)](https://twitter.com/#!/semanticmw)
[![Facebook](https://semantic-mediawiki.org/w/images/thumb/7/77/677166248.png/30px-677166248.png)](https://www.facebook.com/pages/Semantic-MediaWiki/160459700707245)
[![Google+](https://semantic-mediawiki.org/w/images/a/ae/30px-Google%2B.png)](https://plus.google.com/115301028320198614441/posts)

Many people have contributed to SMW. A list of people who have made contributions in the past can
be found [here][contributors] or [on the SMW wiki](https://semantic-mediawiki.org/wiki/Help:SMW_Project#Contributors).
The overview on [how to contribute](https://github.com/SemanticMediaWiki/SemanticMediaWiki/blob/master/CONTRIBUTING.md)
provides information on the different ways available to do so.

If you have remarks, questions, or suggestions, please send them to semediawiki-users@lists.sourceforge.net.
You can subscribe to this list [here](http://sourceforge.net/mailarchive/forum.php?forum_name=semediawiki-user).

If you want to contribute work to the project please subscribe to the developers mailing list and
have a look at the contribution guideline.

* [File an issue](https://github.com/SemanticMediaWiki/SemanticMediaWiki/issues)
* [Submit a pull request](https://github.com/SemanticMediaWiki/SemanticMediaWiki/pulls)
* Ask a question on [the mailing list](https://semantic-mediawiki.org/wiki/Mailing_list)
* Ask a question on the #semantic-mediawiki IRC channel on Freenode.


### Tests

This extension provides unit and integration tests that are normally run by a
[continues integration platform][travis] but tests can also manually be executed using the
`mw-phpunit-runner.php` script or [`phpunit`][mw-testing] together with the PHPUnit configuration
file found in the root directory.

```sh
php mw-phpunit-runner.php [options]
```

## License

[GNU General Public License, version 2 or later][gpl-licence]. The COPYING file explains SMW's copyright and license.

[contributors]: https://github.com/SemanticMediaWiki/SemanticMediaWiki/graphs/contributors
[travis]: https://travis-ci.org/SemanticMediaWiki/SemanticMediaWiki
[mw-testing]: https://www.mediawiki.org/wiki/Manual:PHP_unit_testing
[gpl-licence]: https://www.gnu.org/copyleft/gpl.html
[composer]: https://getcomposer.org/
[smw-installation]: https://www.semantic-mediawiki.org/wiki/Help:Installation
