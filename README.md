Compile plugin for scala.js to output `.d.ts` files.

This project is a placeholder for the moment until I assess how hard this may be
even to do something simple.

Note from gitter: 

The linker sees a very limited version of types, and for exports in particular it sees Anys everywhere. So the linker is definitely not the right place to do that.
The right place to do that is as a compiler plugin that would generate the .d.ts somewhere between the refchecks phase and the erasure phase.
