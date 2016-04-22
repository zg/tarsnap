Client code for Tarsnap
=======================

Tarsnap is a secure, efficient online backup service: "Online
backups for the truly paranoid".

:exclamation: We strongly recommend that people use the latest official
release tarball on https://www.tarsnap.com

> This repository is intended for developers who may wish to watch changes in
> progress or investigate bugs, not for production use.


News
----

A list of major changes in each version is given in [NEWS.md](NEWS.md).


Building from git
-----------------

Normal users should only use the signed tarballs from tarsnap.com,
but for experimental development, use:

    autoreconf -i
    ./configure
    make


Packaging notes
---------------

Bash completion scripts: optional `configure` argument
`--with-bash-completion-dir[=DIR]`.

* If `DIR` is specified, it installs to that directory.

* If `DIR` is left blank, it attempts to use `pkg-config` and
  `bash-completion >= 2.0` to determine where to put the bash
  completion scripts.  If your system does not match those
  requirements, please specify `DIR` explicitly.

