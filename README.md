[![Actions Status](https://github.com/raku-community-modules/vCard-Parser/actions/workflows/linux.yml/badge.svg)](https://github.com/raku-community-modules/vCard-Parser/actions) [![Actions Status](https://github.com/raku-community-modules/vCard-Parser/actions/workflows/macos.yml/badge.svg)](https://github.com/raku-community-modules/vCard-Parser/actions) [![Actions Status](https://github.com/raku-community-modules/vCard-Parser/actions/workflows/windows.yml/badge.svg)](https://github.com/raku-community-modules/vCard-Parser/actions)

NAME
====

vCard::Parser - a basic parser of vCard

SYNOPSIS
========

```perl6
use vCard::Parser;

my $vcard = 'BEGIN:VCARD
VERSION:4.0
N:Gump;Forrest;;Mr.;
x-qq:21588891
END:VCARD';

say from-vCard($vcard);

use JSON::Tiny;
say to-json(from-vCard($vcard)); #Output is jCard
```

DESCRIPTION
===========

vCard::Parser is a basic parser of vCard files of version 4.0. It also serves as it's convertor to jCard, which is a JSON format for vCard data.

AUTHOR
======

Petr Kolář

COPYRIGHT AND LICENSE
=====================

Copyright 2019 Petr Kolář

Copyright 2024 Raku Community

This library is free software; you can redistribute it and/or modify it under the Artistic License 2.0.

