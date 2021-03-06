Read method
===========

Reading a ``csv`` file into a TimeArray object is supported.

readtimearray
-------------

The ``readtimearray`` method is a wrapper for the ``Base.readcsv`` method that returns a TimeArray.

    function readtimearray(fname::String; meta=Nothing, format::String="")

The ``fname`` argument is a string that represents the location and name of the ``csv`` file that you wish to parse into
a TimeArray object. Optionally, you can add a value to the ``meta`` field.

For datetime data that has odd formatting, a ``format`` argument is provided where users can pass the format of their data.

A more robust regex parsing engine is planned so users will not need to pass a time format for anything but the most edge cases.
