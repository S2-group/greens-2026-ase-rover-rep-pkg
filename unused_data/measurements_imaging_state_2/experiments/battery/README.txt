These measurements have been done using 3 services on the pipeline: 
- ambra/energy (0.0.1) -> (modified to send 1 energy message per second)
- ambra/analyser (0.0.2)
- vu-ase/imaging (1.2.4)

The rover has been using a battery. Check first log to see voltage.

Check Imaging.py for setup commands in order to test the experiment.

Each run has 15.8s, same time-length as It would take the rover to drive one lap on the track. Time between runs to cool down is 30 seconds.

!Important!

For this experiment, the rover had an initial temperature of 45 degrees, with 5 degrees more than the cool cpu. It ran fib sequence until it reached 45 degrees

Initial background activity on the rover:
rover08:~ $ ps aux | grep rover
avahi        551  0.0  0.0   7808  3180 ?        Ss   12:48   0:00 avahi-daemon: running 
           [.rover08.local]
root         685  0.0  0.1 627828 12228 ?        Ssl  12:48   0:00 /usr/local/bin/roverd
debix       2945  0.0  0.0   3388  1728 pts/0    S+   12:52   0:00 grep --color=auto rover