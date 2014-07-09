# Webkit dev-tools front-end for Node Webkit Agent

This folder contains code from webkit-devtools-agent-frontend module by Dan MacTough.
More information and source code are available on [NPM](https://www.npmjs.org/package/webkit-devtools-agent-frontend)


## Fork

Official webkit-devtools-agent-frontend module does include both "Profiles" and "Console" tools with minor bugs. This fork slightly modifies the code to provide only remote "Profiles" feature. This fork can easily be spawned as new process with custom agent port passed as argument.


## Example
```javascript
//var agentProfiler = new (global.require('./external/devtools/agent/main'))();
//agentProfiler.start(9999, '0.0.0.0', 3333);

var profiler = require('child_process').spawn('node', ['./external/devtools/profiler/main.js', 9999]);
```


## License
(The BSD License)

Copyright (C) 2013 Terra Eclipse, Inc. (http://www.terraeclipse.com) All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. Neither the name of Terra Eclipse, Inc. nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
