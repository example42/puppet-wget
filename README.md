# Deprecation notice

This module was designed for Puppet versions 2 and 3. It should work also on Puppet 4 but doesn't use any of its features.

The current Puppet 3 compatible codebase is no longer actively maintained by example42.

Still, Pull Requests that fix bugs or introduce backwards compatible features will be accepted.


A Puppet module to download files with wget, supporting authentication.

Example

include wget

wget::fetch { "download":
  source => "http://www.google.com/index.html",
  destination => "/tmp/index.html",
}

wget::fetch { "download":
  source => "http://www.google.com/index.html",
  destination => "/tmp/index.html",
  http_user => "user",
  http_password => "password",
  timeout => 0,
}

[![Build Status](https://travis-ci.org/example42/puppet-wget.png?branch=master)](https://travis-ci.org/example42/puppet-wget)
