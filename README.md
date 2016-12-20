# NAME

Chart::Bokeh - Generate html/javascript charts from perl data using javascript library BokehJS

# VERSION

version 0.001

# SYNOPSIS

```perl
use Chart::Bokeh qw(show_plot);

my $plot_data = {x => [0..10], y => [map {rand 10} 0..10]};

show_plot($plot_data);
```

# DESCRIPTION

Generate html/javascript charts from perl data using javascript library BokehJS. The result
is a file that you could see in your favourite browser.

The interface is "sub" oriented, but the API is subject to changes.

# FUNCTIONS

## render\_full\_html

### Parameters

- data:

    Data to be represented. This early version only accept data as a hashref with keys x, y and arrayrefs as the values:

    ```perl
    { 
      x => [1, 2, 3],
      y => [1, 4, 9]
    }
    ```

## show\_plot

Opens the plot in a browser locally

### Parameters

Data to be represented. The format is the same as the parameter data in render\_full\_html

# DISCLAIMER

This is an unofficial Bokeh Perl module. Currently I'm not affiliated in any way with Bokeh, nor Continuum Analytics, Inc. 
But I think bokeh.js is a great library and I want to use it with perl. Please see: [http://bokeh.pydata.org/en/latest/](http://bokeh.pydata.org/en/latest/)

# AUTHOR

Pablo Rodríguez González <pablo.rodriguez.gonzalez@gmail.com>

# COPYRIGHT AND LICENSE

This software is Copyright (c) 2016 by Pablo Rodríguez González.

This is free software, licensed under:

```perl
The (three-clause) BSD License
```
