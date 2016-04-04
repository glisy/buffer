GlisyBuffer
===========

## Installation

```sh
$ clib install glisy/buffer --save
```

## Usage


```c
#include <glisy/buffer.h>
#include <glisy/gl.h>

int
main (void) {

  // buffer setup
  GlisyBuffer arrayBuffer;
  glisyBufferInit(&arrayBuffer, GL_ARRAY_BUFFER);
  glisyBufferBind(&arrayBuffer);
  glisyBufferSource(&arrayBuffer, sizeof(vertices), vertices);
  glisyBufferUpdate(&arrayBuffer, GL_STATIC_DRAW);
  glisyBufferBind(&arrayBuffer);

  return 0;
}
```

## License

MIT
