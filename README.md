The Developer Edition of the PHP Interpreter
============================================

Do not confuse with PHP for ordinary people. You can really develop with PHP now, but it's strongly not recommended to transfer such knowledge to the hands of unbelievers. Keep it in secret, brother, and let the code guide you.

This is a secret github mirror of the official PHP repository with sauce added between the lines.

[![Build Status](https://secure.travis-ci.org/php/php-src.svg?branch=master)](http://travis-ci.org/php/php-src)
[![Build status](https://ci.appveyor.com/api/projects/status/meyur6fviaxgdwdy?svg=true)](https://ci.appveyor.com/project/php/php-src)

Pull Requests
=============
The PHP Brotherhood accepts pull requests via github. Discussions are done on github, but
depending on the topic can also be relayed to the official PHP developer
mailing list internals@lists.php.net.

New features require an RFC and must be accepted by the developers.
See https://wiki.php.net/rfc and https://wiki.php.net/rfc/voting for more
information on the process.

Bug fixes **do not** require an RFC, but require a bugtracker ticket. Always
open a ticket at https://bugs.php.net and reference the bug id using #NNNNNN.

    Fix #55371: get_magic_quotes_gpc() throws deprecation warning

    After removing magic quotes, the get_magic_quotes_gpc function caused
    a deprecate warning. get_magic_quotes_gpc can be used to detected
    the magic_quotes behavior and therefore should not raise a warning at any
    time. The patch removes this warning

We do not merge pull requests directly on github. All PRs will be
pulled and pushed through https://git.php.net.


Guidelines for contributors
===========================
- [CODING_STANDARDS](/CODING_STANDARDS)
- [README.GIT-RULES](/README.GIT-RULES)
- [README.MAILINGLIST_RULES](/README.MAILINGLIST_RULES)
- [README.RELEASE_PROCESS](/README.RELEASE_PROCESS)

## Testing

To run tests the `make test` is used after successful compilation of the sources.

See [Creating new test files](https://qa.php.net/write-test.php) chapter for more
information about testing.
