# api documentation for  [net-snmp (v1.1.19)](https://github.com/stephenwvickers/node-net-snmp#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-net-snmp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-net-snmp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-net-snmp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-net-snmp)
#### JavaScript implementation of the Simple Network Management Protocol (SNMP)

[![NPM](https://nodei.co/npm/net-snmp.png?downloads=true)](https://www.npmjs.com/package/net-snmp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-net-snmp/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-net-snmp_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-net-snmp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-net-snmp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-net-snmp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stephen Vickers",
        "email": "stephen.vickers.sv@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/stephenwvickers/node-net-snmp/issues"
    },
    "contributors": [
        {
            "name": "Stephen Vickers",
            "email": "stephen.vickers.sv@gmail.com"
        }
    ],
    "dependencies": {
        "asn1": "*"
    },
    "description": "JavaScript implementation of the Simple Network Management Protocol (SNMP)",
    "devDependencies": {},
    "directories": {
        "example": "example"
    },
    "dist": {
        "shasum": "8e08af79fb7b226bd595a4d53aa05eac1329b353",
        "tarball": "https://registry.npmjs.org/net-snmp/-/net-snmp-1.1.19.tgz"
    },
    "gitHead": "cc4860b1b244b9822979d9822056a30e1be6cbb4",
    "homepage": "https://github.com/stephenwvickers/node-net-snmp#readme",
    "keywords": [
        "snmp",
        "snmpv1",
        "snmpv2",
        "snmpv2c",
        "net",
        "network",
        "mon",
        "monitor",
        "monitoring"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "stephen.vickers",
            "email": "stephen.vickers.sv@gmail.com"
        }
    ],
    "name": "net-snmp",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/stephenwvickers/node-net-snmp.git"
    },
    "scripts": {},
    "version": "1.1.19"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module net-snmp](#apidoc.module.net-snmp)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError (message, status)](#apidoc.element.net-snmp.RequestFailedError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError.super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestInvalidError (message)](#apidoc.element.net-snmp.RequestInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestTimedOutError (message)](#apidoc.element.net-snmp.RequestTimedOutError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>ResponseInvalidError (message)](#apidoc.element.net-snmp.ResponseInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>Session (target, community, options)](#apidoc.element.net-snmp.Session)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>createSession (target, community, options)](#apidoc.element.net-snmp.createSession)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>isVarbindError (varbind)](#apidoc.element.net-snmp.isVarbindError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>varbindError (varbind)](#apidoc.element.net-snmp.varbindError)
1.  number <span class="apidocSignatureSpan">net-snmp.</span>Version1
1.  number <span class="apidocSignatureSpan">net-snmp.</span>Version2c
1.  object <span class="apidocSignatureSpan">net-snmp.</span>ErrorStatus
1.  object <span class="apidocSignatureSpan">net-snmp.</span>ObjectParser
1.  object <span class="apidocSignatureSpan">net-snmp.</span>ObjectType
1.  object <span class="apidocSignatureSpan">net-snmp.</span>Session.prototype
1.  object <span class="apidocSignatureSpan">net-snmp.</span>TrapType

#### [module net-snmp.ObjectParser](#apidoc.module.net-snmp.ObjectParser)
1.  [function <span class="apidocSignatureSpan">net-snmp.ObjectParser.</span>readInt (buffer)](#apidoc.element.net-snmp.ObjectParser.readInt)
1.  [function <span class="apidocSignatureSpan">net-snmp.ObjectParser.</span>readUint (buffer, isSigned)](#apidoc.element.net-snmp.ObjectParser.readUint)

#### [module net-snmp.RequestFailedError](#apidoc.module.net-snmp.RequestFailedError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError (message, status)](#apidoc.element.net-snmp.RequestFailedError.RequestFailedError)
1.  [function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.</span>super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_)

#### [module net-snmp.RequestFailedError.super_](#apidoc.module.net-snmp.RequestFailedError.super_)
1.  [function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.</span>super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_.super_)
1.  [function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.super_.</span>captureStackTrace ()](#apidoc.element.net-snmp.RequestFailedError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">net-snmp.RequestFailedError.super_.</span>stackTraceLimit

#### [module net-snmp.RequestInvalidError](#apidoc.module.net-snmp.RequestInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestInvalidError (message)](#apidoc.element.net-snmp.RequestInvalidError.RequestInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.RequestInvalidError.</span>super_ ()](#apidoc.element.net-snmp.RequestInvalidError.super_)

#### [module net-snmp.RequestTimedOutError](#apidoc.module.net-snmp.RequestTimedOutError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>RequestTimedOutError (message)](#apidoc.element.net-snmp.RequestTimedOutError.RequestTimedOutError)
1.  [function <span class="apidocSignatureSpan">net-snmp.RequestTimedOutError.</span>super_ ()](#apidoc.element.net-snmp.RequestTimedOutError.super_)

#### [module net-snmp.ResponseInvalidError](#apidoc.module.net-snmp.ResponseInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>ResponseInvalidError (message)](#apidoc.element.net-snmp.ResponseInvalidError.ResponseInvalidError)
1.  [function <span class="apidocSignatureSpan">net-snmp.ResponseInvalidError.</span>super_ ()](#apidoc.element.net-snmp.ResponseInvalidError.super_)

#### [module net-snmp.Session](#apidoc.module.net-snmp.Session)
1.  [function <span class="apidocSignatureSpan">net-snmp.</span>Session (target, community, options)](#apidoc.element.net-snmp.Session.Session)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.</span>super_ ()](#apidoc.element.net-snmp.Session.super_)

#### [module net-snmp.Session.prototype](#apidoc.module.net-snmp.Session.prototype)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>cancelRequests (error)](#apidoc.element.net-snmp.Session.prototype.cancelRequests)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>close ()](#apidoc.element.net-snmp.Session.prototype.close)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>get (oids, responseCb)](#apidoc.element.net-snmp.Session.prototype.get)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>getBulk ()](#apidoc.element.net-snmp.Session.prototype.getBulk)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>getNext (oids, responseCb)](#apidoc.element.net-snmp.Session.prototype.getNext)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>inform ()](#apidoc.element.net-snmp.Session.prototype.inform)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onClose ()](#apidoc.element.net-snmp.Session.prototype.onClose)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onError (error)](#apidoc.element.net-snmp.Session.prototype.onError)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onMsg (buffer, remote)](#apidoc.element.net-snmp.Session.prototype.onMsg)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onSimpleGetResponse (req, message)](#apidoc.element.net-snmp.Session.prototype.onSimpleGetResponse)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>registerRequest (req)](#apidoc.element.net-snmp.Session.prototype.registerRequest)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>send (req, noWait)](#apidoc.element.net-snmp.Session.prototype.send)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>set (varbinds, responseCb)](#apidoc.element.net-snmp.Session.prototype.set)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>simpleGet (pduClass, feedCb, varbinds, responseCb, options)](#apidoc.element.net-snmp.Session.prototype.simpleGet)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>subtree ()](#apidoc.element.net-snmp.Session.prototype.subtree)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>table ()](#apidoc.element.net-snmp.Session.prototype.table)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>tableColumns ()](#apidoc.element.net-snmp.Session.prototype.tableColumns)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>trap ()](#apidoc.element.net-snmp.Session.prototype.trap)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>unregisterRequest (id)](#apidoc.element.net-snmp.Session.prototype.unregisterRequest)
1.  [function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>walk ()](#apidoc.element.net-snmp.Session.prototype.walk)



# <a name="apidoc.module.net-snmp"></a>[module net-snmp](#apidoc.module.net-snmp)

#### <a name="apidoc.element.net-snmp.RequestFailedError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError (message, status)](#apidoc.element.net-snmp.RequestFailedError)
- description and source-code
```javascript
function RequestFailedError(message, status) {
	this.name = "RequestFailedError";
	this.message = message;
	this.status = status;
	Error.captureStackTrace(this, RequestFailedError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestFailedError.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError.super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestInvalidError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestInvalidError (message)](#apidoc.element.net-snmp.RequestInvalidError)
- description and source-code
```javascript
function RequestInvalidError(message) {
	this.name = "RequestInvalidError";
	this.message = message;
	Error.captureStackTrace(this, RequestInvalidError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestTimedOutError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestTimedOutError (message)](#apidoc.element.net-snmp.RequestTimedOutError)
- description and source-code
```javascript
function RequestTimedOutError(message) {
	this.name = "RequestTimedOutError";
	this.message = message;
	Error.captureStackTrace(this, RequestTimedOutError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.ResponseInvalidError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>ResponseInvalidError (message)](#apidoc.element.net-snmp.ResponseInvalidError)
- description and source-code
```javascript
function ResponseInvalidError(message) {
	this.name = "ResponseInvalidError";
	this.message = message;
	Error.captureStackTrace(this, ResponseInvalidError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>Session (target, community, options)](#apidoc.element.net-snmp.Session)
- description and source-code
```javascript
Session = function (target, community, options) {
	this.target = target || "127.0.0.1";
	this.community = community || "public";

	this.version = (options && options.version)
			? options.version
			: Version1;

	this.transport = (options && options.transport)
			? options.transport
			: "udp4";
	this.port = (options && options.port )
			? options.port
			: 161;
	this.trapPort = (options && options.trapPort )
			? options.trapPort
			: 162;

	this.retries = (options && (options.retries || options.retries == 0))
			? options.retries
			: 1;
	this.timeout = (options && options.timeout)
			? options.timeout
			: 5000;

	this.sourceAddress = (options && options.sourceAddress )
			? options.sourceAddress
			: undefined;
	this.sourcePort = (options && options.sourcePort )
			? parseInt(options.sourcePort)
			: undefined;

	this.reqs = {};
	this.reqCount = 0;

	this.dgram = dgram.createSocket (this.transport);
	this.dgram.unref();
	
	var me = this;
	this.dgram.on ("message", me.onMsg.bind (me));
	this.dgram.on ("close", me.onClose.bind (me));
	this.dgram.on ("error", me.onError.bind (me));

	if (this.sourceAddress || this.sourcePort)
		this.dgram.bind (this.sourcePort, this.sourceAddress);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.createSession"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>createSession (target, community, options)](#apidoc.element.net-snmp.createSession)
- description and source-code
```javascript
createSession = function (target, community, options) {
	return new Session (target, community, options);
}
```
- example usage
```shell
...
## Version 1.1.17 - 21/03/2016

* Correct reference to non-existant 'req' variable in the 'Session' objects
  constructor (should be 'this')

## Version 1.1.18 - 15/05/2015

* Correct argument number and names to the 'snmp.createSession()' function
* Add missing braces to an example in the README.md file

## Version 1.1.19 - 26/08/2016

* Remove 64bit integer check to ensure a maximum of 8 bytes are given in send
  and received messages
...
```

#### <a name="apidoc.element.net-snmp.isVarbindError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>isVarbindError (varbind)](#apidoc.element.net-snmp.isVarbindError)
- description and source-code
```javascript
function isVarbindError(varbind) {
	return !!(varbind.type == ObjectType.NoSuchObject
	|| varbind.type == ObjectType.NoSuchInstance
	|| varbind.type == ObjectType.EndOfMibView);
}
```
- example usage
```shell
...
   error occurred
 * 'varbinds' - Array of varbinds, will not be provided if an error occurred

The varbind in position N in the 'varbinds' array will correspond to the OID
in position N in the 'oids' array in the request.

Each varbind must be checked for an error condition using the
'snmp.isVarbindError()' function when using SNMP version 2c.

The following example fetches values for the sysName ('1.3.6.1.2.1.1.5.0') and
sysLocation ('1.3.6.1.2.1.1.6.0') OIDs:

var oids = ["1.3.6.1.2.1.1.5.0", "1.3.6.1.2.1.1.6.0"];

session.get (oids, function (error, varbinds) {
...
```

#### <a name="apidoc.element.net-snmp.varbindError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>varbindError (varbind)](#apidoc.element.net-snmp.varbindError)
- description and source-code
```javascript
function varbindError(varbind) {
	return (ObjectType[varbind.type] || "NotAnError") + ": " + varbind.oid;
}
```
- example usage
```shell
...
 * 'table' - Object containing object references representing conceptual
   rows keyed by index (e.g. for the ifTable table rows are keyed by ifIndex),
   each row object will contain values keyed by column number, will not be
   provided if an error occurred

If an error occurs with any varbind returned by 'subtree()' no table will be
passed to the 'callback' function.  The reason for failure, and the related
OID string (as returned from a call to the 'snmp.varbindError()' function),
will be passed to the 'callback' function in the 'error' argument as an
instance of the 'RequestFailedError' class.

The following example fetches the ifTable ('1.3.6.1.2.1.2.2') table:

var oid = "1.3.6.1.2.1.2.2";
...
```



# <a name="apidoc.module.net-snmp.ObjectParser"></a>[module net-snmp.ObjectParser](#apidoc.module.net-snmp.ObjectParser)

#### <a name="apidoc.element.net-snmp.ObjectParser.readInt"></a>[function <span class="apidocSignatureSpan">net-snmp.ObjectParser.</span>readInt (buffer)](#apidoc.element.net-snmp.ObjectParser.readInt)
- description and source-code
```javascript
function readInt(buffer) {
	return readUint (buffer, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.ObjectParser.readUint"></a>[function <span class="apidocSignatureSpan">net-snmp.ObjectParser.</span>readUint (buffer, isSigned)](#apidoc.element.net-snmp.ObjectParser.readUint)
- description and source-code
```javascript
function readUint(buffer, isSigned) {
	buffer.readByte ();
	var length = buffer.readByte ();
	var value = 0;
	var signedBitSet = false;

	if (length > 5) {
		 throw new RangeError ("Integer too long '" + length + "'");
	} else if (length == 5) {
		if (buffer.readByte () !== 0)
			throw new RangeError ("Integer too long '" + length + "'");
		length = 4;
	}

	for (var i = 0; i < length; i++) {
		value *= 256;
		value += buffer.readByte ();

		if (isSigned && i <= 0) {
			if ((value & 0x80) == 0x80)
				signedBitSet = true;
		}
	}
	
	if (signedBitSet)
		value -= (1 << (i * 8));

	return value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.RequestFailedError"></a>[module net-snmp.RequestFailedError](#apidoc.module.net-snmp.RequestFailedError)

#### <a name="apidoc.element.net-snmp.RequestFailedError.RequestFailedError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestFailedError (message, status)](#apidoc.element.net-snmp.RequestFailedError.RequestFailedError)
- description and source-code
```javascript
function RequestFailedError(message, status) {
	this.name = "RequestFailedError";
	this.message = message;
	this.status = status;
	Error.captureStackTrace(this, RequestFailedError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestFailedError.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.</span>super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.RequestFailedError.super_"></a>[module net-snmp.RequestFailedError.super_](#apidoc.module.net-snmp.RequestFailedError.super_)

#### <a name="apidoc.element.net-snmp.RequestFailedError.super_.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.</span>super_ ()](#apidoc.element.net-snmp.RequestFailedError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestFailedError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">net-snmp.RequestFailedError.super_.</span>captureStackTrace ()](#apidoc.element.net-snmp.RequestFailedError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
...
/*****************************************************************************
 ** Exception class definitions
 **/

function ResponseInvalidError (message) {
	this.name = "ResponseInvalidError";
	this.message = message;
	Error.captureStackTrace(this, ResponseInvalidError);
}
util.inherits (ResponseInvalidError, Error);

function RequestInvalidError (message) {
	this.name = "RequestInvalidError";
	this.message = message;
	Error.captureStackTrace(this, RequestInvalidError);
...
```



# <a name="apidoc.module.net-snmp.RequestInvalidError"></a>[module net-snmp.RequestInvalidError](#apidoc.module.net-snmp.RequestInvalidError)

#### <a name="apidoc.element.net-snmp.RequestInvalidError.RequestInvalidError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestInvalidError (message)](#apidoc.element.net-snmp.RequestInvalidError.RequestInvalidError)
- description and source-code
```javascript
function RequestInvalidError(message) {
	this.name = "RequestInvalidError";
	this.message = message;
	Error.captureStackTrace(this, RequestInvalidError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestInvalidError.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.RequestInvalidError.</span>super_ ()](#apidoc.element.net-snmp.RequestInvalidError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.RequestTimedOutError"></a>[module net-snmp.RequestTimedOutError](#apidoc.module.net-snmp.RequestTimedOutError)

#### <a name="apidoc.element.net-snmp.RequestTimedOutError.RequestTimedOutError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>RequestTimedOutError (message)](#apidoc.element.net-snmp.RequestTimedOutError.RequestTimedOutError)
- description and source-code
```javascript
function RequestTimedOutError(message) {
	this.name = "RequestTimedOutError";
	this.message = message;
	Error.captureStackTrace(this, RequestTimedOutError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.RequestTimedOutError.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.RequestTimedOutError.</span>super_ ()](#apidoc.element.net-snmp.RequestTimedOutError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.ResponseInvalidError"></a>[module net-snmp.ResponseInvalidError](#apidoc.module.net-snmp.ResponseInvalidError)

#### <a name="apidoc.element.net-snmp.ResponseInvalidError.ResponseInvalidError"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>ResponseInvalidError (message)](#apidoc.element.net-snmp.ResponseInvalidError.ResponseInvalidError)
- description and source-code
```javascript
function ResponseInvalidError(message) {
	this.name = "ResponseInvalidError";
	this.message = message;
	Error.captureStackTrace(this, ResponseInvalidError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.ResponseInvalidError.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.ResponseInvalidError.</span>super_ ()](#apidoc.element.net-snmp.ResponseInvalidError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.Session"></a>[module net-snmp.Session](#apidoc.module.net-snmp.Session)

#### <a name="apidoc.element.net-snmp.Session.Session"></a>[function <span class="apidocSignatureSpan">net-snmp.</span>Session (target, community, options)](#apidoc.element.net-snmp.Session.Session)
- description and source-code
```javascript
Session = function (target, community, options) {
	this.target = target || "127.0.0.1";
	this.community = community || "public";

	this.version = (options && options.version)
			? options.version
			: Version1;

	this.transport = (options && options.transport)
			? options.transport
			: "udp4";
	this.port = (options && options.port )
			? options.port
			: 161;
	this.trapPort = (options && options.trapPort )
			? options.trapPort
			: 162;

	this.retries = (options && (options.retries || options.retries == 0))
			? options.retries
			: 1;
	this.timeout = (options && options.timeout)
			? options.timeout
			: 5000;

	this.sourceAddress = (options && options.sourceAddress )
			? options.sourceAddress
			: undefined;
	this.sourcePort = (options && options.sourcePort )
			? parseInt(options.sourcePort)
			: undefined;

	this.reqs = {};
	this.reqCount = 0;

	this.dgram = dgram.createSocket (this.transport);
	this.dgram.unref();
	
	var me = this;
	this.dgram.on ("message", me.onMsg.bind (me));
	this.dgram.on ("close", me.onClose.bind (me));
	this.dgram.on ("error", me.onError.bind (me));

	if (this.sourceAddress || this.sourcePort)
		this.dgram.bind (this.sourcePort, this.sourceAddress);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.super_"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.</span>super_ ()](#apidoc.element.net-snmp.Session.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.net-snmp.Session.prototype"></a>[module net-snmp.Session.prototype](#apidoc.module.net-snmp.Session.prototype)

#### <a name="apidoc.element.net-snmp.Session.prototype.cancelRequests"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>cancelRequests (error)](#apidoc.element.net-snmp.Session.prototype.cancelRequests)
- description and source-code
```javascript
cancelRequests = function (error) {
	var id;
	for (id in this.reqs) {
		var req = this.reqs[id];
		this.unregisterRequest (req.id);
		req.responseCb (error);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.close"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>close ()](#apidoc.element.net-snmp.Session.prototype.close)
- description and source-code
```javascript
close = function () {
	this.dgram.close ();
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.get"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>get (oids, responseCb)](#apidoc.element.net-snmp.Session.prototype.get)
- description and source-code
```javascript
get = function (oids, responseCb) {
	function feedCb (req, message) {
		var pdu = message.pdu;
		var varbinds = [];

		if (req.message.pdu.varbinds.length != pdu.varbinds.length) {
			req.responseCb (new ResponseInvalidError ("Requested OIDs do not "
					+ "match response OIDs"));
		} else {
			for (var i = 0; i < req.message.pdu.varbinds.length; i++) {
				if (req.message.pdu.varbinds[i].oid != pdu.varbinds[i].oid) {
					req.responseCb (new ResponseInvalidError ("OID '"
							+ req.message.pdu.varbinds[i].oid
							+ "' in request at positiion '" + i + "' does not "
							+ "match OID '" + pdu.varbinds[i].oid + "' in response "
							+ "at position '" + i + "'"));
					return;
				} else {
					varbinds.push (pdu.varbinds[i]);
				}
			}

			req.responseCb (null, varbinds);
		}
	}

	var pduVarbinds = [];

	for (var i = 0; i < oids.length; i++) {
		var varbind = {
			oid: oids[i]
		};
		pduVarbinds.push (varbind);
	}

	this.simpleGet (GetRequestPdu, feedCb, pduVarbinds, responseCb);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.getBulk"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>getBulk ()](#apidoc.element.net-snmp.Session.prototype.getBulk)
- description and source-code
```javascript
getBulk = function () {
	var oids, nonRepeaters, maxRepetitions, responseCb;

	if (arguments.length >= 4) {
		oids = arguments[0];
		nonRepeaters = arguments[1];
		maxRepetitions = arguments[2];
		responseCb = arguments[3];
	} else if (arguments.length >= 3) {
		oids = arguments[0];
		nonRepeaters = arguments[1];
		maxRepetitions = 10;
		responseCb = arguments[2];
	} else {
		oids = arguments[0];
		nonRepeaters = 0;
		maxRepetitions = 10;
		responseCb = arguments[1];
	}

	function feedCb (req, message) {
		var pdu = message.pdu;
		var varbinds = [];
		var i = 0;

		// first walk through and grab non-repeaters
		if (pdu.varbinds.length < nonRepeaters) {
			req.responseCb (new ResponseInvalidError ("Varbind count in "
					+ "response '" + pdu.varbinds.length + "' is less than "
					+ "non-repeaters '" + nonRepeaters + "' in request"));
		} else {
			for ( ; i < nonRepeaters; i++) {
				if (isVarbindError (pdu.varbinds[i])) {
					varbinds.push (pdu.varbinds[i]);
				} else if (! oidFollowsOid (req.message.pdu.varbinds[i].oid,
						pdu.varbinds[i].oid)) {
					req.responseCb (new ResponseInvalidError ("OID '"
							+ req.message.pdu.varbinds[i].oid + "' in request at "
							+ "positiion '" + i + "' does not precede "
							+ "OID '" + pdu.varbinds[i].oid + "' in response "
							+ "at position '" + i + "'"));
					return;
				} else {
					varbinds.push (pdu.varbinds[i]);
				}
			}
		}

		var repeaters = req.message.pdu.varbinds.length - nonRepeaters;

		// secondly walk through and grab repeaters
		if (pdu.varbinds.length % (repeaters)) {
			req.responseCb (new ResponseInvalidError ("Varbind count in "
					+ "response '" + pdu.varbinds.length + "' is not a "
					+ "multiple of repeaters '" + repeaters
					+ "' plus non-repeaters '" + nonRepeaters + "' in request"));
		} else {
			while (i < pdu.varbinds.length) {
				for (var j = 0; j < repeaters; j++, i++) {
					var reqIndex = nonRepeaters + j;
					var respIndex = i;

					if (isVarbindError (pdu.varbinds[respIndex])) {
						if (! varbinds[reqIndex])
							varbinds[reqIndex] = [];
						varbinds[reqIndex].push (pdu.varbinds[respIndex]);
					} else if (! oidFollowsOid (
							req.message.pdu.varbinds[reqIndex].oid,
							pdu.varbinds[respIndex].oid)) {
						req.responseCb (new ResponseInvalidError ("OID '"
								+ req.message.pdu.varbinds[reqIndex].oid
								+ "' in request at positiion '" + (reqIndex)
								+ "' does not precede OID '"
								+ pdu.varbinds[respIndex].oid
								+ "' in response at position '" + (respIndex) + "'"));
						return;
					} else {
						if (! varbinds[reqIndex])
							varbinds[reqIndex] = [];
						varbinds[reqIndex].push (pdu.varbinds[respIndex]);
					}
				}
			}
		}

		req.responseCb (null, varbinds);
	}

	var pduVarbinds = [];

	for (var i = 0; i < oids.length; i++) {
		var varbind = {
			oid: oids[i]
		};
		pduVarbinds.push (varbind);
	}

	var options = {
		nonRepeaters: nonRepeaters,
		maxRepetitions: maxRepetitions
	};

	this.simpleGet (GetBulkRequestPdu, feedCb, pduVarbinds, responseCb,
			options);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.getNext"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>getNext (oids, responseCb)](#apidoc.element.net-snmp.Session.prototype.getNext)
- description and source-code
```javascript
getNext = function (oids, responseCb) {
	function feedCb (req, message) {
		var pdu = message.pdu;
		var varbinds = [];

		if (req.message.pdu.varbinds.length != pdu.varbinds.length) {
			req.responseCb (new ResponseInvalidError ("Requested OIDs do not "
					+ "match response OIDs"));
		} else {
			for (var i = 0; i < req.message.pdu.varbinds.length; i++) {
				if (isVarbindError (pdu.varbinds[i])) {
					varbinds.push (pdu.varbinds[i]);
				} else if (! oidFollowsOid (req.message.pdu.varbinds[i].oid,
						pdu.varbinds[i].oid)) {
					req.responseCb (new ResponseInvalidError ("OID '"
							+ req.message.pdu.varbinds[i].oid + "' in request at "
							+ "positiion '" + i + "' does not precede "
							+ "OID '" + pdu.varbinds[i].oid + "' in response "
							+ "at position '" + i + "'"));
					return;
				} else {
					varbinds.push (pdu.varbinds[i]);
				}
			}

			req.responseCb (null, varbinds);
		}
	}

	var pduVarbinds = [];

	for (var i = 0; i < oids.length; i++) {
		var varbind = {
			oid: oids[i]
		};
		pduVarbinds.push (varbind);
	}

	this.simpleGet (GetNextRequestPdu, feedCb, pduVarbinds, responseCb);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.inform"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>inform ()](#apidoc.element.net-snmp.Session.prototype.inform)
- description and source-code
```javascript
inform = function () {
	var typeOrOid = arguments[0];
	var varbinds, options = {}, responseCb;

	<span class="apidocCodeCommentSpan">/**
	 ** Support the following signatures:
	 **
	 **    typeOrOid, varbinds, options, callback
	 **    typeOrOid, varbinds, callback
	 **    typeOrOid, options, callback
	 **    typeOrOid, callback
	 **/
</span>	if (arguments.length >= 4) {
		varbinds = arguments[1];
		options = arguments[2];
		responseCb = arguments[3];
	} else if (arguments.length >= 3) {
		if (arguments[1].constructor != Array) {
			varbinds = [];
			options = arguments[1];
			responseCb = arguments[2];
		} else {
			varbinds = arguments[1];
			responseCb = arguments[2];
		}
	} else {
		varbinds = [];
		responseCb = arguments[1];
	}

	function feedCb (req, message) {
		var pdu = message.pdu;
		var varbinds = [];

		if (req.message.pdu.varbinds.length != pdu.varbinds.length) {
			req.responseCb (new ResponseInvalidError ("Inform OIDs do not "
					+ "match response OIDs"));
		} else {
			for (var i = 0; i < req.message.pdu.varbinds.length; i++) {
				if (req.message.pdu.varbinds[i].oid != pdu.varbinds[i].oid) {
					req.responseCb (new ResponseInvalidError ("OID '"
							+ req.message.pdu.varbinds[i].oid
							+ "' in inform at positiion '" + i + "' does not "
							+ "match OID '" + pdu.varbinds[i].oid + "' in response "
							+ "at position '" + i + "'"));
					return;
				} else {
					varbinds.push (pdu.varbinds[i]);
				}
			}

			req.responseCb (null, varbinds);
		}
	}

	if (typeof typeOrOid != "string")
		typeOrOid = "1.3.6.1.6.3.1.1.5." + (typeOrOid + 1);

	var pduVarbinds = [
		{
			oid: "1.3.6.1.2.1.1.3.0",
			type: ObjectType.TimeTicks,
			value: options.upTime || Math.floor (process.uptime () * 100)
		},
		{
			oid: "1.3.6.1.6.3.1.1.4.1.0",
			type: ObjectType.OID,
			value: typeOrOid
		}
	];

	for (var i = 0; i < varbinds.length; i++) {
		var varbind = {
			oid: varbinds[i].oid,
			type: varbinds[i].type,
			value: varbinds[i].value
		};
		pduVarbinds.push (varbind);
	}
	
	options.port = this.trapPort;

	this.simpleGet (InformRequestPdu, feedCb, pduVarbinds, responseCb, options);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.onClose"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onClose ()](#apidoc.element.net-snmp.Session.prototype.onClose)
- description and source-code
```javascript
onClose = function () {
	this.cancelRequests (new Error ("Socket forcibly closed"));
	this.emit ("close");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.onError"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onError (error)](#apidoc.element.net-snmp.Session.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
	this.emit (error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.onMsg"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onMsg (buffer, remote)](#apidoc.element.net-snmp.Session.prototype.onMsg)
- description and source-code
```javascript
onMsg = function (buffer, remote) {
	try {
		var message = new ResponseMessage (buffer);

		var req = this.unregisterRequest (message.pdu.id);
		if (! req)
			return;

		try {
			if (message.version != req.message.version) {
				req.responseCb (new ResponseInvalidError ("Version in request '"
						+ req.message.version + "' does not match version in "
						+ "response '" + message.version));
			} else if (message.community != req.message.community) {
				req.responseCb (new ResponseInvalidError ("Community '"
						+ req.message.community + "' in request does not match "
						+ "community '" + message.community + "' in response"));
			} else if (message.pdu.type == PduType.GetResponse) {
				req.onResponse (req, message);
			} else {
				req.responseCb (new ResponseInvalidError ("Unknown PDU type '"
						+ message.pdu.type + "' in response"));
			}
		} catch (error) {
			req.responseCb (error);
		}
	} catch (error) {
		this.emit("error", error);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.onSimpleGetResponse"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>onSimpleGetResponse (req, message)](#apidoc.element.net-snmp.Session.prototype.onSimpleGetResponse)
- description and source-code
```javascript
onSimpleGetResponse = function (req, message) {
	var pdu = message.pdu;

	if (pdu.errorStatus > 0) {
		var statusString = ErrorStatus[pdu.errorStatus]
				|| ErrorStatus.GeneralError;
		var statusCode = ErrorStatus[statusString]
				|| ErrorStatus[ErrorStatus.GeneralError];

		if (pdu.errorIndex <= 0 || pdu.errorIndex > pdu.varbinds.length) {
			req.responseCb (new RequestFailedError (statusString, statusCode));
		} else {
			var oid = pdu.varbinds[pdu.errorIndex - 1].oid;
			var error = new RequestFailedError (statusString + ": " + oid,
					statusCode);
			req.responseCb (error);
		}
	} else {
		req.feedCb (req, message);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.registerRequest"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>registerRequest (req)](#apidoc.element.net-snmp.Session.prototype.registerRequest)
- description and source-code
```javascript
registerRequest = function (req) {
	if (! this.reqs[req.id]) {
		this.reqs[req.id] = req;
		if (this.reqCount <= 0)
			this.dgram.ref();
		this.reqCount++;
	}
	var me = this;
	req.timer = setTimeout (function () {
		if (req.retries-- > 0) {
			me.send (req);
		} else {
			me.unregisterRequest (req.id);
			req.responseCb (new RequestTimedOutError (
					"Request timed out"));
		}
	}, req.timeout);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.send"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>send (req, noWait)](#apidoc.element.net-snmp.Session.prototype.send)
- description and source-code
```javascript
send = function (req, noWait) {
	try {
		var me = this;
		
		var buffer = req.message.toBuffer ();

		this.dgram.send (buffer, 0, buffer.length, req.port, this.target,
				function (error, bytes) {
			if (error) {
				req.responseCb (error);
			} else {
				if (noWait) {
					req.responseCb (null);
				} else {
					me.registerRequest (req);
				}
			}
		});
	} catch (error) {
		req.responseCb (error);
	}
	
	return this;
}
```
- example usage
```shell
...
* Corrected a few instances of the parameter named 'requestCallback' to some
  methods in the README.md file which should have been 'feedCallback'
* Null type is used for varbinds with a 0 value
* Correct instances of snmp.Type to snmp.ObjectType in the README.md file

## Version 1.1.10 - 01/12/2013

* Error handler in the 'dgram.send()' callback in the 'send()' method was
  creating a new instance of the 'Error' class from the 'error' parameter, but
  it was already an instance of the 'Error' class (thanks Ray Solomon)
* Add stack traces to Error classes exported by this module (thanks Ray
  Solomon)
* Allow users to specify '0' retries when creating a session (thanks Ray
  Solomon)
* Update the list of SNMP version 1 related RFCs we adhere to in the
...
```

#### <a name="apidoc.element.net-snmp.Session.prototype.set"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>set (varbinds, responseCb)](#apidoc.element.net-snmp.Session.prototype.set)
- description and source-code
```javascript
set = function (varbinds, responseCb) {
	function feedCb (req, message) {
		var pdu = message.pdu;
		var varbinds = [];

		if (req.message.pdu.varbinds.length != pdu.varbinds.length) {
			req.responseCb (new ResponseInvalidError ("Requested OIDs do not "
					+ "match response OIDs"));
		} else {
			for (var i = 0; i < req.message.pdu.varbinds.length; i++) {
				if (req.message.pdu.varbinds[i].oid != pdu.varbinds[i].oid) {
					req.responseCb (new ResponseInvalidError ("OID '"
							+ req.message.pdu.varbinds[i].oid
							+ "' in request at positiion '" + i + "' does not "
							+ "match OID '" + pdu.varbinds[i].oid + "' in response "
							+ "at position '" + i + "'"));
					return;
				} else {
					varbinds.push (pdu.varbinds[i]);
				}
			}

			req.responseCb (null, varbinds);
		}
	}

	var pduVarbinds = [];

	for (var i = 0; i < varbinds.length; i++) {
		var varbind = {
			oid: varbinds[i].oid,
			type: varbinds[i].type,
			value: varbinds[i].value
		};
		pduVarbinds.push (varbind);
	}

	this.simpleGet (SetRequestPdu, feedCb, pduVarbinds, responseCb);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.simpleGet"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>simpleGet (pduClass, feedCb, varbinds, responseCb, options)](#apidoc.element.net-snmp.Session.prototype.simpleGet)
- description and source-code
```javascript
simpleGet = function (pduClass, feedCb, varbinds, responseCb, options) {
	var req = {};

	try {
		var id = _generateId ();
		var pdu = new pduClass (id, varbinds, options);
		var message = new RequestMessage (this.version, this.community, pdu);

		req = {
			id: id,
			message: message,
			responseCb: responseCb,
			retries: this.retries,
			timeout: this.timeout,
			onResponse: this.onSimpleGetResponse,
			feedCb: feedCb,
			port: (options && options.port) ? options.port : this.port
		};

		this.send (req);
	} catch (error) {
		if (req.responseCb)
			req.responseCb (error);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.subtree"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>subtree ()](#apidoc.element.net-snmp.Session.prototype.subtree)
- description and source-code
```javascript
subtree = function () {
	var me = this;
	var oid = arguments[0];
	var maxRepetitions, feedCb, doneCb;

	if (arguments.length < 4) {
		maxRepetitions = 20;
		feedCb = arguments[1];
		doneCb = arguments[2];
	} else {
		maxRepetitions = arguments[1];
		feedCb = arguments[2];
		doneCb = arguments[3];
	}

	var req = {
		feedCb: feedCb,
		doneCb: doneCb,
		maxRepetitions: maxRepetitions,
		baseOid: oid
	};

	this.walk (oid, maxRepetitions, subtreeCb.bind (me, req), doneCb);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.table"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>table ()](#apidoc.element.net-snmp.Session.prototype.table)
- description and source-code
```javascript
table = function () {
	var me = this;

	var oid = arguments[0];
	var maxRepetitions, responseCb;

	if (arguments.length < 3) {
		responseCb = arguments[1];
		maxRepetitions = 20;
	} else {
		maxRepetitions = arguments[1];
		responseCb = arguments[2];
	}

	var req = {
		responseCb: responseCb,
		maxRepetitions: maxRepetitions,
		baseOid: oid,
		rowOid: oid + ".1.",
		table: {}
	};

	this.subtree (oid, maxRepetitions, tableFeedCb.bind (me, req),
			tableResponseCb.bind (me, req));

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.tableColumns"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>tableColumns ()](#apidoc.element.net-snmp.Session.prototype.tableColumns)
- description and source-code
```javascript
tableColumns = function () {
	var me = this;

	var oid = arguments[0];
	var columns = arguments[1];
	var maxRepetitions, responseCb;

	if (arguments.length < 4) {
		responseCb = arguments[2];
		maxRepetitions = 20;
	} else {
		maxRepetitions = arguments[2];
		responseCb = arguments[3];
	}

	var req = {
		responseCb: responseCb,
		maxRepetitions: maxRepetitions,
		baseOid: oid,
		rowOid: oid + ".1.",
		columns: columns.slice(0),
		table: {}
	};

	if (req.columns.length > 0) {
		var column = req.columns.pop ();
		this.subtree (req.rowOid + column, maxRepetitions,
				tableColumnsFeedCb.bind (me, req),
				tableColumnsResponseCb.bind (me, req));
	}

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.trap"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>trap ()](#apidoc.element.net-snmp.Session.prototype.trap)
- description and source-code
```javascript
trap = function () {
	var req = {};

	try {
		var typeOrOid = arguments[0];
		var varbinds, options = {}, responseCb;

		<span class="apidocCodeCommentSpan">/**
		 ** Support the following signatures:
		 **
		 **    typeOrOid, varbinds, options, callback
		 **    typeOrOid, varbinds, agentAddr, callback
		 **    typeOrOid, varbinds, callback
		 **    typeOrOid, agentAddr, callback
		 **    typeOrOid, options, callback
		 **    typeOrOid, callback
		 **/
</span>		if (arguments.length >= 4) {
			varbinds = arguments[1];
			if (typeof arguments[2] == "string") {
				options.agentAddr = arguments[2];
			} else if (arguments[2].constructor != Array) {
				options = arguments[2];
			}
			responseCb = arguments[3];
		} else if (arguments.length >= 3) {
			if (typeof arguments[1] == "string") {
				varbinds = [];
				options.agentAddr = arguments[1];
			} else if (arguments[1].constructor != Array) {
				varbinds = [];
				options = arguments[1];
			} else {
				varbinds = arguments[1];
				agentAddr = null;
			}
			responseCb = arguments[2];
		} else {
			varbinds = [];
			responseCb = arguments[1];
		}

		var pdu, pduVarbinds = [];

		for (var i = 0; i < varbinds.length; i++) {
			var varbind = {
				oid: varbinds[i].oid,
				type: varbinds[i].type,
				value: varbinds[i].value
			};
			pduVarbinds.push (varbind);
		}
		
		var id = _generateId ();

		if (this.version == Version2c) {
			if (typeof typeOrOid != "string")
				typeOrOid = "1.3.6.1.6.3.1.1.5." + (typeOrOid + 1);

			pduVarbinds.unshift (
				{
					oid: "1.3.6.1.2.1.1.3.0",
					type: ObjectType.TimeTicks,
					value: options.upTime || Math.floor (process.uptime () * 100)
				},
				{
					oid: "1.3.6.1.6.3.1.1.4.1.0",
					type: ObjectType.OID,
					value: typeOrOid
				}
			);

			pdu = new TrapV2Pdu (id, pduVarbinds, options);
		} else {
			pdu = new TrapPdu (typeOrOid, pduVarbinds, options);
		}

		var message = new RequestMessage (this.version, this.community, pdu);

		req = {
			id: id,
			message: message,
			responseCb: responseCb,
			port: this.trapPort
		};

		this.send (req, true);
	} catch (error) {
		if (req.responseCb)
			req.responseCb (error);
	}

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.unregisterRequest"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>unregisterRequest (id)](#apidoc.element.net-snmp.Session.prototype.unregisterRequest)
- description and source-code
```javascript
unregisterRequest = function (id) {
	var req = this.reqs[id];
	if (req) {
		delete this.reqs[id];
		clearTimeout (req.timer);
		delete req.timer;
		this.reqCount--;
		if (this.reqCount <= 0)
			this.dgram.unref();
		return req;
	} else {
		return null;
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.net-snmp.Session.prototype.walk"></a>[function <span class="apidocSignatureSpan">net-snmp.Session.prototype.</span>walk ()](#apidoc.element.net-snmp.Session.prototype.walk)
- description and source-code
```javascript
walk = function () {
	var me = this;
	var oid = arguments[0];
	var maxRepetitions, feedCb, doneCb, baseOid;

	if (arguments.length < 4) {
		maxRepetitions = 20;
		feedCb = arguments[1];
		doneCb = arguments[2];
	} else {
		maxRepetitions = arguments[1];
		feedCb = arguments[2];
		doneCb = arguments[3];
	}

	var req = {
		maxRepetitions: maxRepetitions,
		feedCb: feedCb,
		doneCb: doneCb
	};

	if (this.version == Version2c)
		this.getBulk ([oid], 0, maxRepetitions,
				walkCb.bind (me, req));
	else
		this.getNext ([oid], walkCb.bind (me, req));

	return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
