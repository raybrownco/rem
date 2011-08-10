rem() is a Sass mixin that converts pixel values to rem values for whatever property is passed to it.
It returns two lines of code — one of the regular pixel values (for some older browsers), and another with the
converted rem values (for everyone else). Special thanks to Chris Epstein (http://chriseppstein.github.com)
and Martin Bavio (http://martinbavio.com) for the help and code!

_Sample input:_

    .element {
      @include rem('padding',10px 0 2px 5px);
    }

_Sample output:_

    .element {
      padding: 10px 0 2px 5px;
      padding: 1rem 0 0.2rem 0.5rem;
    }