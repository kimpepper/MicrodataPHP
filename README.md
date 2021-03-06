MicrodataPHP [![Build Status](https://travis-ci.org/linclark/MicrodataPHP.svg?branch=2.0.x)](https://travis-ci.org/linclark/MicrodataPHP)
============

Microdata is a syntax for embedding machine-readable metadata in HTML.

MicrodataPHP is a PHP library for extracting microdata from HTML documents. It
is inspired by MicrodataJS, which is inspired by the native Microdata DOM API.

Example use:
```
  $url = 'http://lin-clark.com/cool-hand-luke';
  $md = new MicrodataPhp($url);
  $data = $md->obj();
  print $data->items[0]->properties['name'][0];   //prints 'Cool Hand Luke'
  print $data->items[0]->properties['genre'][0];  //prints 'prison drama'
```

Requirements
============

PHP 5.3+
