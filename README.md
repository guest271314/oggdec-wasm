# oggdec-wasm

Decode ogg files in the browser using vorbis tools' oggdec via emscripten.

Build it from scratch by just downloading the Makefile and pre.js, run make, and then:

```
import module from "./oggdec"
const Module = module()
const decodeOggData = Module.decodeOggData
const decodedData = decodeOggData([...some array buffer...])
```

(Compiles on Mac, not tested on Linux)
