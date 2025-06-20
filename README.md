# 62541demo
using https://github.com/open62541/open62541 as submodule to make an example

```bash
git submodule update --init --recursive
mkdir build
cd build
cmake ../open62541
make

```

to build examples

```
sudo make install
cp ../open62541/examples/tutorial_server_firststeps.c .
gcc -std=c99 -o server tutorial_server_firststeps.c -lopen62541
```

Now to figure out what all of this means. I also want to do otel with this. I think that I need https://github.com/dorsal-lab/opentelemetry-c.
