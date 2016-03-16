URI objects are handy things for manipulating URLs.  They let you parse and resolve URIs quickly and easily.  e.g.

```
  var some_uri = new URI("http://www.example.com/foo/bar");

  alert(some_uri.authority); // www.example.com
  alert(some_uri);           // http://www.example.com/foo/bar

  var blah      = new URI("blah");
  var blah_full = blah.resolve(some_uri);
  alert(blah_full);         // http://www.example.com/foo/blah
```

This library is inspired by Perl's URI.pm.