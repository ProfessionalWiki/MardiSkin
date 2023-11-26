# MardiSkin

## Dependencies

Install [Chameleon skin](https://github.com/ProfessionalWiki/chameleon/), at least version 4.3.0.

## Installation
Clone this repo into `skins/MardiSkin`.

Add the following to `LocalSettings.php`:
```php
wfLoadExtension( 'Bootstrap' );
wfLoadskin( 'chameleon' );
$wgDefaultSkin = 'chameleon';
$egChameleonLayoutFile= __DIR__ . '/skins/MardiSkin/layout.xml';
$egChameleonExternalStyleModules = [
	__DIR__ . '/skins/MardiSkin/variables.scss' => 'beforeVariables',
	__DIR__ . '/skins/MardiSkin/styles.scss' => 'afterMain',
];
```
