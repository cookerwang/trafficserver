.. Licensed to the Apache Software Foundation (ASF) under one or more
   contributor license agreements.  See the NOTICE file distributed
   with this work for additional information regarding copyright
   ownership.  The ASF licenses this file to you under the Apache
   License, Version 2.0 (the "License"); you may not use this file
   except in compliance with the License.  You may obtain a copy of
   the License at

      http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
   implied.  See the License for the specific language governing
   permissions and limitations under the License.


TSUrlDestroy
============

Destroys the URL located at url_loc within the marshal buffer bufp.


Synopsis
--------

`#include <ts/ts.h>`

.. c:function:: TSReturnCode TSUrlDestroy(TSMBuffer bufp, TSMLoc offset)


Description
-----------

Do not forget to release the :c:type:`TSMLoc` url_loc with a call to
:c:func:`TSHandleMLocRelease`.

.. admonition:: Deprecated

   There is no reason to destroy the URL, just release the marshal
   buffers.

Should be removed for v5.0.0
