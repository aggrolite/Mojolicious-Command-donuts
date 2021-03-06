# NAME

Mojolicious::Command::donuts - Find fresh donuts with Mojolicious!

# SYNOPSIS

    $ mojo donuts --geo 34.14,-118.40 --fresh
    $ mojo donuts --raw
    $ mojo donuts

# DESCRIPTION

Mojolicious::Command::donuts currently only fetches results
from KrispyKreme. If geo is not specified, this module tries
to geocode your IP and use that for searching.

The fresh option filters results by stores which have their
"Hotlight" on. This means fresh donuts.

The raw option prints out the raw data structure returned from
the site (currently KripsyKreme). If --raw is not enabled,
The store's address is printed out along with any Hotlight
indicator.

# TODO

This module was written with the intent of supporting
more than one donuts site - e.g. Yum Yum and Dunkin Donuts.
Unfortunately, those sites make it a bit more difficult
to scrape results. However, patches are welcome!

# AUTHOR

Curtis Brandt &lt;curtis@cpan.org>

# COPYRIGHT

Copyright 2015- Curtis Brandt

# LICENSE

The (two-clause) FreeBSD License. See LICENSE for details.

# SEE ALSO

[WWW::KrispyKreme::HotLight](https://metacpan.org/pod/WWW::KrispyKreme::HotLight)
