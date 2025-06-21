# 62541demo
using https://github.com/open62541/open62541 as submodule to make an example

```bash
git submodule update --init --recursive
mkdir build
cd build
cmake ../open62541
make

```

to build examples from https://www.open62541.org/doc/master/tutorials.html.

```
sudo make install
cd ../tutorial
gcc -std=c99 -o server tutorial_server_firststeps.c -lopen62541
```

There are lots more examples in `../open62541/examples`.

Now to figure out what all of this means. I also want to do otel with this. I think that I need https://github.com/dorsal-lab/opentelemetry-c.

I also have nginx unit installed. To run unit in the foreground `sudo unitd --no-daemon`.
