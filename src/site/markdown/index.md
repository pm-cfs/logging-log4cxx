<!--
 Licensed to the Apache Software Foundation (ASF) under one or more
 contributor license agreements.  See the NOTICE file distributed with
 this work for additional information regarding copyright ownership.
 The ASF licenses this file to You under the Apache License, Version 2.0
 (the "License"); you may not use this file except in compliance with
 the License.  You may obtain a copy of the License at

	http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-->

# Short introduction to Apache log4cxx

Apache log4cxx is a logging framework for C++ patterned after [Apache log4j],
which uses [Apache Portable Runtime] for most platform-specific code and should
be usable on any platform supported by APR. Apache log4cxx is licensed under
the [Apache License], an open source license certified by the [Open Source Initiative].

Almost every large application includes its own logging or tracing API.
Inserting log statements into code is a low-tech method for debugging it.
It may also be the only way because debuggers are not always available or
applicable. This is usually the case for multithreaded applications and distributed
applications at large.

Experience indicates that logging is an important component of the development
cycle. It offers several advantages. It provides precise context about a run of
the application. Once inserted into the code, the generation of logging output
requires no human intervention. Moreover, log output can be saved in persistent
medium to be studied at a later time. In addition to its use in the development
cycle, a sufficiently rich logging package can also be viewed as an auditing tool.

Logging does have its drawbacks. It can slow down an application. If too verbose,
it can cause scrolling blindness. To alleviate these concerns, log4cxx is
designed to be reliable, fast and extensible. Since logging is rarely the
main focus of an application, the log4cxx API strives to be simple to
understand and to use.

[Apache log4j]:https://logging.apache.org/log4j/2.x/
[Apache Portable Runtime]:https://apr.apache.org/
[Apache License]:https://www.apache.org/licenses/
[Open Source Initiative]:https://opensource.org/
