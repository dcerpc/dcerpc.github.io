---
title: Source
redirect_from: /source.html
---

## Getting and Building the Source

The DCE/RPC source code is available from [GitHub](https://github.com/dcerpc/dcerpc):

    ~ $ git clone https://github.com/dcerpc/dcerpc.git dcerpc.git

To build the project on macOS, use the Xcode project. This will
build the DCERPC framework and the `dceidl` IDL compiler, which is
all that is necessary to start writing DCE/RPC applications.
   
    ~/dcerpc.git $ cd dcerpc
    ~/dcerpc.git $ ./bootstrap
    ~/dcerpc.git $ cd ..
    ~/dcerpc.git $ xcodebuild -configuration Debug -target dceidl
    ~/dcerpc.git $ sudo xcodebuild -configuration Debug -target dceidl install DSTROOT=/
    ~/dcerpc.git $ xcodebuild -configuration Debug -target DCERPC

To build on Linux or other UNIX-like systems, use the autotools
build system.

    ~/dcerpc.git $ cd dcerpc
    ~/dcerpc.git $ autoreconf -fi
    ~/dcerpc.git $ ./configure && make
    ~/dcerpc.git $ sudo make install

## Licensing

DCE/RPC is licensed under the following terms:

    Copyright (c) 2010 Apple Inc. All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:

    1.  Redistributions of source code must retain the above copyright
        notice, this list of conditions and the following disclaimer.
    2.  Redistributions in binary form must reproduce the above copyright
        notice, this list of conditions and the following disclaimer in the
        documentation and/or other materials provided with the distribution.
    3.  Neither the name of Apple Inc. ("Apple") nor the names of its
        contributors may be used to endorse or promote products derived from
        this software without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY APPLE AND ITS CONTRIBUTORS "AS IS" AND ANY
    EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
    DISCLAIMED. IN NO EVENT SHALL APPLE OR ITS CONTRIBUTORS BE LIABLE FOR ANY
    DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
    (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
    ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
    THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

    (c) Copyright 1989-1993 OPEN SOFTWARE FOUNDATION, INC.
    (c) Copyright 1989-1993 HEWLETT-PACKARD COMPANY
    (c) Copyright 1989-1993 DIGITAL EQUIPMENT CORPORATION
    To anyone who acknowledges that this file is provided "AS IS"
    without any express or implied warranty:
                    permission to use, copy, modify, and distribute this
    file for any purpose is hereby granted without fee, provided that
    the above copyright notices and this notice appears in all source
    code copies, and that none of the names of Open Software
    Foundation, Inc., Hewlett-Packard Company, or Digital Equipment
    Corporation be used in advertising or publicity pertaining to
    distribution of the software without specific, written prior
    permission.  Neither Open Software Foundation, Inc., Hewlett-
    Packard Company, nor Digital Equipment Corporation makes any
    representations about the suitability of this software for any
    purpose.

    Copyright (c) 2007, Novell, Inc.
    All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:
    1. Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
    3. Neither the name of the Novell, Inc. nor the names of its contributors
       may be used to endorse or promote products derived from this software
       without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
    "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
    LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
    A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
    OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
    SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
    LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
    DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
    THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

    The following is applicable to ncklib/com/cominit_ux.c:

    Copyright (c) 1983, 1993
           The Regents of the University of California.  All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:
    1. Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
    3. All advertising materials mentioning features or use of this software
       must display the following acknowledgement:
           This product includes software developed by the University of
           California, Berkeley and its contributors.
    4. Neither the name of the University nor the names of its contributors
       may be used to endorse or promote products derived from this software
       without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY THE REGENTS AND CONTRIBUTORS ``AS IS'' AND
    ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
    ARE DISCLAIMED.  IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE
    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
    OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
    HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
    LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
    OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
    SUCH DAMAGE.

    The following is applicable to uuid/get_802_addr.c:

    The OpenLDAP Public License
      Version 2.8, 17 August 2003

    Redistribution and use of this software and associated documentation
    ("Software"), with or without modification, are permitted provided
    that the following conditions are met:

    1. Redistributions in source form must retain copyright statements
       and notices,

    2. Redistributions in binary form must reproduce applicable copyright
       statements and notices, this list of conditions, and the following
       disclaimer in the documentation and/or other materials provided
       with the distribution, and

    3. Redistributions must contain a verbatim copy of this document.

    The OpenLDAP Foundation may revise this license from time to time.
    Each revision is distinguished by a version number.  You may use
    this Software under terms of this license revision or under the
    terms of any subsequent revision of the license.

    THIS SOFTWARE IS PROVIDED BY THE OPENLDAP FOUNDATION AND ITS
    CONTRIBUTORS ``AS IS'' AND ANY EXPRESSED OR IMPLIED WARRANTIES,
    INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY
    AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT
    SHALL THE OPENLDAP FOUNDATION, ITS CONTRIBUTORS, OR THE AUTHOR(S)
    OR OWNER(S) OF THE SOFTWARE BE LIABLE FOR ANY DIRECT, INDIRECT,
    INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
    BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
    LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
    ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
    POSSIBILITY OF SUCH DAMAGE.

    The names of the authors and copyright holders must not be used in
    advertising or otherwise to promote the sale, use or other dealing
    in this Software without specific, written prior permission.  Title
    to copyright in this Software shall at all times remain with copyright
    holders.

    OpenLDAP is a registered trademark of the OpenLDAP Foundation.

    Copyright 1999-2003 The OpenLDAP Foundation, Redwood City,
    California, USA.  All Rights Reserved.  Permission to copy and
    distribute verbatim copies of this document is granted.
