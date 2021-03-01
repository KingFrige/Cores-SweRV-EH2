README
=========

generate all the equations below from "csrdecode" except legal equation:

```
$ cp ../design/dec/csrdecode
$ ./coredecode -in csrdecode > corecsrdecode.e
$ ./espresso -Dso -oeqntott corecsrdecode.e | ./addassign  > csrequations
```

generate the legal CSR equation below:

```
# ./coredecode -in csrdecode -legal > csrlegal.e
# ./espresso -Dso -oeqntott csrlegal.e | ./addassign  > csrlegal_equation
```

reference
--------------

[Espresso](http://www.ecs.umass.edu/ece/labs/vlsicad/ece667/links/espresso.html)


