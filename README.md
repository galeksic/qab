# qab

Quick ab.c

This is http://gwan.com/source/ab.c (http://gwan.com/en_apachebench_httperf.html), with defaults sligthly lowered.

```
// default range and number of requests
int  FROM = 0, TO = 100, STEP = 10, ITER = 3;
// int  FROM = 0, TO = 1000, STEP = 10, ITER = 3;
int  NBR_REQUESTS = 2000;
// int  NBR_REQUESTS = 100000;
```

That's why it is "quick".

Build:

```
gcc -O2 qab.c -o qabc -lpthread
```

Make it available just for you or at the system level. (Optional, of course.)

```
mv qabc ~/bin
```

```
sudo chown root:root qabc
sudo mv qabc /usr/local/bin
```
