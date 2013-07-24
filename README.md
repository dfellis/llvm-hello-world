# llvm-hello-world

Simple repo for figuring out how to write and compile llvm assembler.

## Notes

This is based almost entirely on the example in the LLVM documentation, but had to modify it slightly as the example wouldn't compile.

Thankfully the compiler gives really good warning and error messages. :)

## How To

LLVM includes an LLVM Assembler interpreter, ``lli``. After installing LLVM (I have version 3.3) simply type:

```bash
lli helloWorld.ll
```

There's also a compiler that converts the LLVM assembly into x86 (or whatever your local arch is) assembly, ``llc``:

```bash
llc helloWorld.ll # Creates helloWorld.s
```

I've included my output assembly for reference.

## License (UoI/NCSA)

    Copyright (c) 2013 David Ellis
    All rights reserved.
    
    Developed by:     David Ellis and LLVM
                      http://dfellis.github.io/
    
    Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal with the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
    
    Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimers.
    Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimers in the documentation and/or other materials provided with the distribution.
    Neither the names of David Ellis and LLVM, nor the names of its contributors may be used to endorse or promote products derived from this Software without specific prior written permission. 
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE CONTRIBUTORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS WITH THE SOFTWARE. 