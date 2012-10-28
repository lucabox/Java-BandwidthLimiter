Java BandwidthLimiter
=====================

A simple class allowing to register Input/Output streams in order to limit the bandwidth at which they can
read or send each second.

Features
--------

- setting a maximum read (e.g. download if you register a socket's stream) bandwidth
- setting a maximum write (e.g. upload if you register a socket's stream) bandwidth
- adding some additional latency that the streams will suffer of.


Note
----

the bandwidth assigned to each stream is a first in first gets it basis, no attempt so far has been done
to mimic a "fair" behaviour, if you'd like to implement this features I have left pointers in the code
on where this should be handled (and feel free to contribute back! :) )


TODO
----

- Add some examples/tests (e.g. using with custom socket factories)
- Investigate whether it's possible to adapt this class in order to limit Java NIO classes too.

