#EasySlug

##Description
EasySlug is very simple class to making slug from base text.

##Instalation
Using Composer, just require the pyton/easyslug package:

```json
{
    "require": {
        "pyton/easyslug": "dev-master"
    }
}
```

##Usage
```php
$easySlug = new EasySlug();

$string = 'Base Slug string.';
$slug = $easySlug->create($string);

echo $slug->plain() . PHP_EOL;
// base-slug-string

echo $slug->format('%s.html') . PHP_EOL;
// base-slug-string.html

$easySlug->setReplacement('_');
$slug = $easySlug->create($string);
echo $slug->plain() . PHP_EOL;
// base_slug_string

echo $slug->format('%s.html') . PHP_EOL;
// base_slug_string.html
```

##Credits
Łukasz Piotrowski <lukasz@piotrows.pl>