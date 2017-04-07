# api documentation for  [ssh2 (v0.5.4)](https://github.com/mscdex/ssh2#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ssh2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ssh2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ssh2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ssh2)
#### SSH2 client and server modules written in pure JavaScript for node.js

[![NPM](https://nodei.co/npm/ssh2.png?downloads=true)](https://www.npmjs.com/package/ssh2)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ssh2/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-ssh2%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ssh2/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ssh2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ssh2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian White",
        "email": "mscdex@mscdex.net"
    },
    "bugs": {
        "url": "https://github.com/mscdex/ssh2/issues"
    },
    "dependencies": {
        "ssh2-streams": "~0.1.15"
    },
    "description": "SSH2 client and server modules written in pure JavaScript for node.js",
    "devDependencies": {
        "semver": "^5.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1bf6b6b28c96eaef267f4d6c46a5a2517a599e27",
        "tarball": "https://registry.npmjs.org/ssh2/-/ssh2-0.5.4.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "homepage": "https://github.com/mscdex/ssh2#readme",
    "keywords": [
        "ssh",
        "ssh2",
        "sftp",
        "secure",
        "shell",
        "exec",
        "remote",
        "client"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://github.com/mscdex/ssh2/raw/master/LICENSE"
        }
    ],
    "main": "./lib/client",
    "maintainers": [
        {
            "name": "mscdex",
            "email": "mscdex@mscdex.net"
        }
    ],
    "name": "ssh2",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/mscdex/ssh2.git"
    },
    "scripts": {
        "test": "node test/test.js"
    },
    "version": "0.5.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ssh2](#apidoc.module.ssh2)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>Channel (info, client, opts)](#apidoc.element.ssh2.Channel)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>Client ()](#apidoc.element.ssh2.Client)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>SFTPWrapper (stream)](#apidoc.element.ssh2.SFTPWrapper)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>Server (cfg, listener)](#apidoc.element.ssh2.Server)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>keepalivemgr (interval, streamInterval, kaCountMax)](#apidoc.element.ssh2.keepalivemgr)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>super_ ()](#apidoc.element.ssh2.super_)
1.  object <span class="apidocSignatureSpan">ssh2.</span>Channel.prototype
1.  object <span class="apidocSignatureSpan">ssh2.</span>SFTPWrapper.prototype
1.  object <span class="apidocSignatureSpan">ssh2.</span>SFTP_OPEN_MODE
1.  object <span class="apidocSignatureSpan">ssh2.</span>SFTP_STATUS_CODE
1.  object <span class="apidocSignatureSpan">ssh2.</span>Server.prototype
1.  object <span class="apidocSignatureSpan">ssh2.</span>keepalivemgr.prototype
1.  object <span class="apidocSignatureSpan">ssh2.</span>utils

#### [module ssh2.Channel](#apidoc.module.ssh2.Channel)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>Channel (info, client, opts)](#apidoc.element.ssh2.Channel.Channel)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.</span>super_ (options)](#apidoc.element.ssh2.Channel.super_)
1.  number <span class="apidocSignatureSpan">ssh2.Channel.</span>MAX_WINDOW
1.  number <span class="apidocSignatureSpan">ssh2.Channel.</span>PACKET_SIZE

#### [module ssh2.Channel.prototype](#apidoc.module.ssh2.Channel.prototype)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>_read (n)](#apidoc.element.ssh2.Channel.prototype._read)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>_write (data, encoding, cb)](#apidoc.element.ssh2.Channel.prototype._write)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>close ()](#apidoc.element.ssh2.Channel.prototype.close)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>destroy ()](#apidoc.element.ssh2.Channel.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>eof ()](#apidoc.element.ssh2.Channel.prototype.eof)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>exit (name, coreDumped, msg)](#apidoc.element.ssh2.Channel.prototype.exit)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>setWindow (rows, cols, height, width)](#apidoc.element.ssh2.Channel.prototype.setWindow)
1.  [function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>signal (signalName)](#apidoc.element.ssh2.Channel.prototype.signal)

#### [module ssh2.SFTPWrapper](#apidoc.module.ssh2.SFTPWrapper)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>SFTPWrapper (stream)](#apidoc.element.ssh2.SFTPWrapper.SFTPWrapper)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.</span>super_ ()](#apidoc.element.ssh2.SFTPWrapper.super_)

#### [module ssh2.SFTPWrapper.prototype](#apidoc.module.ssh2.SFTPWrapper.prototype)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>appendFile (path, data, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.appendFile)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>chmod (path, mode, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.chmod)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>chown (path, uid, gid, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.chown)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>close (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.close)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>createReadStream (path, options)](#apidoc.element.ssh2.SFTPWrapper.prototype.createReadStream)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>createWriteStream (path, options)](#apidoc.element.ssh2.SFTPWrapper.prototype.createWriteStream)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>end ()](#apidoc.element.ssh2.SFTPWrapper.prototype.end)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>exists (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.exists)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_fstatvfs (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fstatvfs)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_fsync (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fsync)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_hardlink (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_hardlink)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_rename (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_rename)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_statvfs (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_statvfs)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fastGet (remotePath, localPath, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fastGet)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fastPut (localPath, remotePath, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fastPut)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fchmod (handle, mode, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fchmod)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fchown (handle, uid, gid, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fchown)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fsetstat (handle, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fsetstat)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fstat (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fstat)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>futimes (handle, atime, mtime, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.futimes)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>lstat (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.lstat)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>mkdir (path, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.mkdir)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>open (path, flags, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.open)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>opendir (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.opendir)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>read (handle, buf, off, len, position, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.read)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readFile (path, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.readFile)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readdir (where, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.readdir)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readlink (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.readlink)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>realpath (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.realpath)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>rename (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.rename)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>rmdir (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.rmdir)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>setstat (path, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.setstat)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>stat (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.stat)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>symlink (targetPath, linkPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.symlink)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>unlink (filename, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.unlink)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>utimes (path, atime, mtime, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.utimes)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>write (handle, buf, off, len, position, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.write)
1.  [function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>writeFile (path, data, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.writeFile)

#### [module ssh2.Server](#apidoc.module.ssh2.Server)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>Server (cfg, listener)](#apidoc.element.ssh2.Server.Server)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.</span>createServer (cfg, listener)](#apidoc.element.ssh2.Server.createServer)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.</span>super_ ()](#apidoc.element.ssh2.Server.super_)
1.  number <span class="apidocSignatureSpan">ssh2.Server.</span>KEEPALIVE_CLIENT_COUNT_MAX
1.  number <span class="apidocSignatureSpan">ssh2.Server.</span>KEEPALIVE_CLIENT_INTERVAL
1.  number <span class="apidocSignatureSpan">ssh2.Server.</span>KEEPALIVE_INTERVAL

#### [module ssh2.Server.prototype](#apidoc.module.ssh2.Server.prototype)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>address ()](#apidoc.element.ssh2.Server.prototype.address)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>close (cb)](#apidoc.element.ssh2.Server.prototype.close)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>getConnections (cb)](#apidoc.element.ssh2.Server.prototype.getConnections)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>listen ()](#apidoc.element.ssh2.Server.prototype.listen)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>ref ()](#apidoc.element.ssh2.Server.prototype.ref)
1.  [function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>unref ()](#apidoc.element.ssh2.Server.prototype.unref)

#### [module ssh2.keepalivemgr](#apidoc.module.ssh2.keepalivemgr)
1.  [function <span class="apidocSignatureSpan">ssh2.</span>keepalivemgr (interval, streamInterval, kaCountMax)](#apidoc.element.ssh2.keepalivemgr.keepalivemgr)

#### [module ssh2.keepalivemgr.prototype](#apidoc.module.ssh2.keepalivemgr.prototype)
1.  [function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>add (stream)](#apidoc.element.ssh2.keepalivemgr.prototype.add)
1.  [function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>remove (stream)](#apidoc.element.ssh2.keepalivemgr.prototype.remove)
1.  [function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>start ()](#apidoc.element.ssh2.keepalivemgr.prototype.start)
1.  [function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>stop ()](#apidoc.element.ssh2.keepalivemgr.prototype.stop)

#### [module ssh2.utils](#apidoc.module.ssh2.utils)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>DSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.DSAKeySSHToASN1)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>DSASigBERToBare (signature)](#apidoc.element.ssh2.utils.DSASigBERToBare)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>DSASigBareToBER (signature)](#apidoc.element.ssh2.utils.DSASigBareToBER)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.ECDSAKeySSHToASN1)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSASigASN1ToSSH (signature)](#apidoc.element.ssh2.utils.ECDSASigASN1ToSSH)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSASigSSHToASN1 (signature, self, callback)](#apidoc.element.ssh2.utils.ECDSASigSSHToASN1)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>RSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.RSAKeySSHToASN1)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>convertPPKPrivate (keyInfo)](#apidoc.element.ssh2.utils.convertPPKPrivate)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>decryptKey (keyInfo, passphrase)](#apidoc.element.ssh2.utils.decryptKey)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>genPublicKey (keyInfo)](#apidoc.element.ssh2.utils.genPublicKey)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>isStreamCipher (name)](#apidoc.element.ssh2.utils.isStreamCipher)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>iv_inc (iv)](#apidoc.element.ssh2.utils.iv_inc)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>parseKey (data)](#apidoc.element.ssh2.utils.parseKey)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>readInt (buffer, start, stream, cb)](#apidoc.element.ssh2.utils.readInt)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>readString (buffer, start, encoding, stream, cb, maxLen)](#apidoc.element.ssh2.utils.readString)
1.  [function <span class="apidocSignatureSpan">ssh2.utils.</span>verifyPPKMAC (keyInfo, passphrase, privateKey)](#apidoc.element.ssh2.utils.verifyPPKMAC)



# <a name="apidoc.module.ssh2"></a>[module ssh2](#apidoc.module.ssh2)

#### <a name="apidoc.element.ssh2.Channel"></a>[function <span class="apidocSignatureSpan">ssh2.</span>Channel (info, client, opts)](#apidoc.element.ssh2.Channel)
- description and source-code
```javascript
function Channel(info, client, opts) {
  var streamOpts = {
    highWaterMark: MAX_WINDOW,
    allowHalfOpen: (!opts || (opts && opts.allowHalfOpen !== false))
  };

  this.allowHalfOpen = streamOpts.allowHalfOpen;

  DuplexStream.call(this, streamOpts);

  var self = this;
  var server = opts && opts.server;

  this.server = server;
  this.type = info.type;
  this.subtype = undefined;
<span class="apidocCodeCommentSpan">  /*
    incoming and outgoing contain these properties:
    {
      id: undefined,
      window: undefined,
      packetSize: undefined,
      state: 'closed'
    }
  */
</span>  var incoming = this.incoming = info.incoming;
  var incomingId = incoming.id;
  var outgoing = this.outgoing = info.outgoing;
  var callbacks = this._callbacks = [];
  var exitCode;
  var exitSignal;
  var exitDump;
  var exitDesc;
  var exitLang;

  this._client = client;
  this._hasX11 = false;

  var channels = client._channels;
  var sshstream = client._sshstream;

  function ondrain() {
    if (self._waitClientDrain) {
      self._waitClientDrain = false;
      if (!self._waitWindow) {
        if (self._chunk)
          self._write(self._chunk, null, self._chunkcb);
        else if (self._chunkcb)
          self._chunkcb();
        else if (self._chunkErr)
          self.stderr._write(self._chunkErr, null, self._chunkcbErr);
        else if (self._chunkcbErr)
          self._chunkcbErr();
      }
    }
  }
  client._sock.on('drain', ondrain);

  sshstream.once('CHANNEL_EOF:' + incomingId, function() {
    if (incoming.state === 'closed' || incoming.state === 'eof')
      return;
    incoming.state = 'eof';

    if (self.readable)
      self.push(null);
    if (!server && self.stderr.readable)
      self.stderr.push(null);
  }).once('CHANNEL_CLOSE:' + incomingId, function() {
    if (incoming.state === 'closed')
      return;
    incoming.state = 'closed';

    if (self.readable)
      self.push(null);
    if (server && self.stderr.writable)
      self.stderr.end();
    else if (!server && self.stderr.readable)
      self.stderr.push(null);

    if (outgoing.state === 'open' || outgoing.state === 'eof')
      self.close();
    if (outgoing.state === 'closing')
      outgoing.state = 'closed';

    delete channels[incomingId];

    var state = self._writableState;
    client._sock.removeListener('drain', ondrain);
    if (!state.ending && !state.finished)
      self.end();

    // Take care of any outstanding channel requests
    self._callbacks = [];
    for (var i = 0; i < callbacks.length; ++i)
      callbacks[i](true);
    callbacks = self._callbacks;

    if (!server) {
      // align more with node child processes, where the close event gets the
      // same arguments as the exit event
      if (!self.readable) {
        if (exitCode === null) {
          self.emit('close', exitCode, exitSignal, exitDump, exitDesc,
                    exitLang);
        } else
          self.emit('close', exitCode);
      } else {
        self.once('end', function() {
          if (exitCode === null) {
            self.emit('close', exitCode, exitSignal, exitDump, exitDesc,
                      exitLang);
          } else
            self.emit('close', exitCode);
        });
      }

      if (!self.stderr.readable)
        self.stderr.emit('close');
      else {
        self.stderr.once('end', function() {
          self.stderr.emit('close');
        });
      }
    } else { // Server mode
      if (!self.readable)
        self.emit('close');
      else {
        self.once('end', function() {
          self.emit('close');
        });
      }
    }

    for (var i = 0; i < CUSTOM_EVENTS_LEN; ++i)
      sshstream.removeAllListeners(CUSTOM_EVENTS[i] + ':' + incomingId);
  }).on('CHANNEL_DATA:' + incomingId, function(data) {
    // the remote party should not be sending us data if there is no window
    // space available ...
    if (incoming.window === 0)
      return;

    incoming.window -= data.length;

    if (!self.push(data)) {
      self._waitChanDrain = true;
      return;
    }

    if (incoming.window <= WINDOW_THRESHOLD)
      windowAdjust(self);
  }).on('CHANNEL_WIN ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Client"></a>[function <span class="apidocSignatureSpan">ssh2.</span>Client ()](#apidoc.element.ssh2.Client)
- description and source-code
```javascript
function Client() {
  if (!(this instanceof Client))
    return new Client();

  EventEmitter.call(this);

  this.config = {
    host: undefined,
    port: undefined,
    forceIPv4: undefined,
    forceIPv6: undefined,
    keepaliveCountMax: undefined,
    keepaliveInterval: undefined,
    readyTimeout: undefined,

    username: undefined,
    password: undefined,
    privateKey: undefined,
    publicKey: undefined,
    tryKeyboard: undefined,
    agent: undefined,
    allowAgentFwd: undefined,

    hostHashAlgo: undefined,
    hostHashCb: undefined,
    strictVendor: undefined,
    debug: undefined
  };

  this._readyTimeout = undefined;
  this._channels = undefined;
  this._callbacks = undefined;
  this._forwarding = undefined;
  this._acceptX11 = undefined;
  this._agentFwdEnabled = undefined;
  this._curChan = undefined;
  this._remoteVer = undefined;

  this._sshstream = undefined;
  this._sock = undefined;
  this._resetKA = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.SFTPWrapper"></a>[function <span class="apidocSignatureSpan">ssh2.</span>SFTPWrapper (stream)](#apidoc.element.ssh2.SFTPWrapper)
- description and source-code
```javascript
function SFTPWrapper(stream) {
  var self = this;

  EventEmitter.call(this);

  this._stream = stream;

  stream.on('error', function(err) {
    self.emit('error', err);
  }).on('end', function() {
    self.emit('end');
  }).on('close', function() {
    self.emit('close');
  }).on('continue', function() {
    self.emit('continue');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Server"></a>[function <span class="apidocSignatureSpan">ssh2.</span>Server (cfg, listener)](#apidoc.element.ssh2.Server)
- description and source-code
```javascript
function Server(cfg, listener) {
  if (!(this instanceof Server))
    return new Server(cfg, listener);

  var hostKeys = {
    'ssh-rsa': null,
    'ssh-dss': null,
    'ecdsa-sha2-nistp256': null,
    'ecdsa-sha2-nistp384': null,
    'ecdsa-sha2-nistp521': null
  };

  var hostKeys_ = cfg.hostKeys;
  if (!Array.isArray(hostKeys_))
    throw new Error('hostKeys must be an array');

  var i;
  for (i = 0; i < hostKeys_.length; ++i) {
    var privateKey;
    if (Buffer.isBuffer(hostKeys_[i]) || typeof hostKeys_[i] === 'string')
      privateKey = parseKey(hostKeys_[i]);
    else
      privateKey = parseKey(hostKeys_[i].key);
    if (privateKey instanceof Error)
      throw new Error('Cannot parse privateKey: ' + privateKey.message);
    if (!privateKey.private)
      throw new Error('privateKey value contains an invalid private key');
    if (hostKeys[privateKey.fulltype])
      continue;
    if (privateKey.encryption) {
      if (typeof hostKeys_[i].passphrase !== 'string')
        throw new Error('Missing passphrase for encrypted private key');
      decryptKey(privateKey, hostKeys_[i].passphrase);
    }
    hostKeys[privateKey.fulltype] = {
      privateKey: privateKey,
      publicKey: genPublicKey(privateKey)
    };
  }

  var algorithms = {
    kex: undefined,
    kexBuf: undefined,
    cipher: undefined,
    cipherBuf: undefined,
    serverHostKey: undefined,
    serverHostKeyBuf: undefined,
    hmac: undefined,
    hmacBuf: undefined,
    compress: undefined,
    compressBuf: undefined
  };
  if (typeof cfg.algorithms === 'object' && cfg.algorithms !== null) {
    var algosSupported;
    var algoList;

    algoList = cfg.algorithms.kex;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_KEX;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported key exchange algorithm: ' + algoList[i]);
      }
      algorithms.kex = algoList;
    }

    algoList = cfg.algorithms.cipher;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_CIPHER;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported cipher algorithm: ' + algoList[i]);
      }
      algorithms.cipher = algoList;
    }

    algoList = cfg.algorithms.serverHostKey;
    var copied = false;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_SERVER_HOST_KEY;
      for (i = algoList.length - 1; i >= 0; --i) {
        if (algosSupported.indexOf(algoList[i]) === -1) {
          throw new Error('Unsupported server host key algorithm: '
                           + algoList[i]);
        }
        if (!hostKeys[algoList[i]]) {
          // Silently discard for now
          if (!copied) {
            algoList = algoList.slice();
            copied = true;
          }
          algoList.splice(i, 1);
        }
      }
      if (algoList.length > 0)
        algorithms.serverHostKey = algoList;
    }

    algoList = cfg.algorithms.hmac;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_HMAC;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported HMAC algorithm: ' + algoList[i]);
      }
      algorithms.hmac = algoList;
    }

    algoList = cfg.algorithms.compress;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_COMPRESS;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported compression algorithm: ' + algoList[i]);
      }
      algorithms.compress = algoList;
    }
  }

  // Make sure we at least have some kind of valid list of support key
  // formats
  if (algorithms.serverHostKey === undefined) {
    var hostKeyAlgos = Object.keys(hostKeys);
    for (i = hostKeyAlgos.length - 1; i ...
```
- example usage
```shell
...

var buffersEqual = require('buffer-equal-constant-time');
var ssh2 = require('ssh2');
var utils = ssh2.utils;

var pubKey = utils.genPublicKey(utils.parseKey(fs.readFileSync('user.pub')));

new ssh2.Server({
hostKeys: [fs.readFileSync('host.key')]
}, function(client) {
console.log('Client connected!');

client.on('authentication', function(ctx) {
  if (ctx.method === 'password'
      && ctx.username === 'foo'
...
```

#### <a name="apidoc.element.ssh2.keepalivemgr"></a>[function <span class="apidocSignatureSpan">ssh2.</span>keepalivemgr (interval, streamInterval, kaCountMax)](#apidoc.element.ssh2.keepalivemgr)
- description and source-code
```javascript
function Manager(interval, streamInterval, kaCountMax) {
  var streams = this._streams = [];
  this._timer = undefined;
  this._timerInterval = interval;
  this._timerfn = function() {
    var now = Date.now();
    for (var i = 0, len = streams.length, s, last; i < len; ++i) {
      s = streams[i];
      last = s._kalast;
      if (last && (now - last) >= streamInterval) {
        if (++s._kacnt > kaCountMax) {
          var err = new Error('Keepalive timeout');
          err.level = 'client-timeout';
          s.emit('error', err);
          s.disconnect();
          spliceOne(streams, i);
          --i;
          len = streams.length;
        } else {
          s._kalast = now;
          // XXX: if the server ever starts sending real global requests to the
          //      client, we will need to add a dummy callback here to keep the
          //      correct reply order
          s.ping();
        }
      }
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.super_"></a>[function <span class="apidocSignatureSpan">ssh2.</span>super_ ()](#apidoc.element.ssh2.super_)
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



# <a name="apidoc.module.ssh2.Channel"></a>[module ssh2.Channel](#apidoc.module.ssh2.Channel)

#### <a name="apidoc.element.ssh2.Channel.Channel"></a>[function <span class="apidocSignatureSpan">ssh2.</span>Channel (info, client, opts)](#apidoc.element.ssh2.Channel.Channel)
- description and source-code
```javascript
function Channel(info, client, opts) {
  var streamOpts = {
    highWaterMark: MAX_WINDOW,
    allowHalfOpen: (!opts || (opts && opts.allowHalfOpen !== false))
  };

  this.allowHalfOpen = streamOpts.allowHalfOpen;

  DuplexStream.call(this, streamOpts);

  var self = this;
  var server = opts && opts.server;

  this.server = server;
  this.type = info.type;
  this.subtype = undefined;
<span class="apidocCodeCommentSpan">  /*
    incoming and outgoing contain these properties:
    {
      id: undefined,
      window: undefined,
      packetSize: undefined,
      state: 'closed'
    }
  */
</span>  var incoming = this.incoming = info.incoming;
  var incomingId = incoming.id;
  var outgoing = this.outgoing = info.outgoing;
  var callbacks = this._callbacks = [];
  var exitCode;
  var exitSignal;
  var exitDump;
  var exitDesc;
  var exitLang;

  this._client = client;
  this._hasX11 = false;

  var channels = client._channels;
  var sshstream = client._sshstream;

  function ondrain() {
    if (self._waitClientDrain) {
      self._waitClientDrain = false;
      if (!self._waitWindow) {
        if (self._chunk)
          self._write(self._chunk, null, self._chunkcb);
        else if (self._chunkcb)
          self._chunkcb();
        else if (self._chunkErr)
          self.stderr._write(self._chunkErr, null, self._chunkcbErr);
        else if (self._chunkcbErr)
          self._chunkcbErr();
      }
    }
  }
  client._sock.on('drain', ondrain);

  sshstream.once('CHANNEL_EOF:' + incomingId, function() {
    if (incoming.state === 'closed' || incoming.state === 'eof')
      return;
    incoming.state = 'eof';

    if (self.readable)
      self.push(null);
    if (!server && self.stderr.readable)
      self.stderr.push(null);
  }).once('CHANNEL_CLOSE:' + incomingId, function() {
    if (incoming.state === 'closed')
      return;
    incoming.state = 'closed';

    if (self.readable)
      self.push(null);
    if (server && self.stderr.writable)
      self.stderr.end();
    else if (!server && self.stderr.readable)
      self.stderr.push(null);

    if (outgoing.state === 'open' || outgoing.state === 'eof')
      self.close();
    if (outgoing.state === 'closing')
      outgoing.state = 'closed';

    delete channels[incomingId];

    var state = self._writableState;
    client._sock.removeListener('drain', ondrain);
    if (!state.ending && !state.finished)
      self.end();

    // Take care of any outstanding channel requests
    self._callbacks = [];
    for (var i = 0; i < callbacks.length; ++i)
      callbacks[i](true);
    callbacks = self._callbacks;

    if (!server) {
      // align more with node child processes, where the close event gets the
      // same arguments as the exit event
      if (!self.readable) {
        if (exitCode === null) {
          self.emit('close', exitCode, exitSignal, exitDump, exitDesc,
                    exitLang);
        } else
          self.emit('close', exitCode);
      } else {
        self.once('end', function() {
          if (exitCode === null) {
            self.emit('close', exitCode, exitSignal, exitDump, exitDesc,
                      exitLang);
          } else
            self.emit('close', exitCode);
        });
      }

      if (!self.stderr.readable)
        self.stderr.emit('close');
      else {
        self.stderr.once('end', function() {
          self.stderr.emit('close');
        });
      }
    } else { // Server mode
      if (!self.readable)
        self.emit('close');
      else {
        self.once('end', function() {
          self.emit('close');
        });
      }
    }

    for (var i = 0; i < CUSTOM_EVENTS_LEN; ++i)
      sshstream.removeAllListeners(CUSTOM_EVENTS[i] + ':' + incomingId);
  }).on('CHANNEL_DATA:' + incomingId, function(data) {
    // the remote party should not be sending us data if there is no window
    // space available ...
    if (incoming.window === 0)
      return;

    incoming.window -= data.length;

    if (!self.push(data)) {
      self._waitChanDrain = true;
      return;
    }

    if (incoming.window <= WINDOW_THRESHOLD)
      windowAdjust(self);
  }).on('CHANNEL_WIN ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Channel.super_"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.</span>super_ (options)](#apidoc.element.ssh2.Channel.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ssh2.Channel.prototype"></a>[module ssh2.Channel.prototype](#apidoc.module.ssh2.Channel.prototype)

#### <a name="apidoc.element.ssh2.Channel.prototype._read"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>_read (n)](#apidoc.element.ssh2.Channel.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  if (this._waitChanDrain) {
    this._waitChanDrain = false;
    if (this.incoming.window <= WINDOW_THRESHOLD)
      windowAdjust(this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Channel.prototype._write"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>_write (data, encoding, cb)](#apidoc.element.ssh2.Channel.prototype._write)
- description and source-code
```javascript
_write = function (data, encoding, cb) {
  var sshstream = this._client._sshstream;
  var outgoing = this.outgoing;
  var packetSize = outgoing.packetSize;
  var id = outgoing.id;
  var window = outgoing.window;
  var len = data.length;
  var p = 0;
  var ret;
  var buf;
  var sliceLen;

  if (outgoing.state !== 'open')
    return;

  while (len - p > 0 && window > 0) {
    sliceLen = len - p;
    if (sliceLen > window)
      sliceLen = window;
    if (sliceLen > packetSize)
      sliceLen = packetSize;

    ret = sshstream.channelData(id, data.slice(p, p + sliceLen));

    p += sliceLen;
    window -= sliceLen;

    if (!ret) {
      this._waitClientDrain = true;
      this._chunk = undefined;
      this._chunkcb = cb;
      break;
    }
  }

  outgoing.window = window;

  if (len - p > 0) {
    if (window === 0)
      this._waitWindow = true;
    if (p > 0) {
      // partial
      buf = new Buffer(len - p);
      data.copy(buf, 0, p);
      this._chunk = buf;
    } else
      this._chunk = data;
    this._chunkcb = cb;
    return;
  }

  if (!this._waitClientDrain)
    cb();
}
```
- example usage
```shell
...
var sshstream = client._sshstream;

function ondrain() {
  if (self._waitClientDrain) {
    self._waitClientDrain = false;
    if (!self._waitWindow) {
      if (self._chunk)
        self._write(self._chunk, null, self._chunkcb);
      else if (self._chunkcb)
        self._chunkcb();
      else if (self._chunkErr)
        self.stderr._write(self._chunkErr, null, self._chunkcbErr);
      else if (self._chunkcbErr)
        self._chunkcbErr();
    }
...
```

#### <a name="apidoc.element.ssh2.Channel.prototype.close"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>close ()](#apidoc.element.ssh2.Channel.prototype.close)
- description and source-code
```javascript
close = function () {
  var ret = true;
  var outgoing = this.outgoing;

  if (outgoing.state === 'open' || outgoing.state === 'eof') {
    outgoing.state = 'closing';
    ret = this._client._sshstream.channelClose(outgoing.id);
  }

  return ret;
}
```
- example usage
```shell
...
  self.push(null);
if (server && self.stderr.writable)
  self.stderr.end();
else if (!server && self.stderr.readable)
  self.stderr.push(null);

if (outgoing.state === 'open' || outgoing.state === 'eof')
  self.close();
if (outgoing.state === 'closing')
  outgoing.state = 'closed';

delete channels[incomingId];

var state = self._writableState;
client._sock.removeListener('drain', ondrain);
...
```

#### <a name="apidoc.element.ssh2.Channel.prototype.destroy"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>destroy ()](#apidoc.element.ssh2.Channel.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.end();
}
```
- example usage
```shell
...
      sig = new Buffer(siglen);
      count = 0;
    }
  } else {
    sig[count] = chunk[i];
    if (++count === siglen) {
      sock.removeAllListeners('data');
      return sock.destroy();
    }
  }
} else if (type === IDENTITIES_ANSWER) {
  /*
    byte        SSH2_AGENT_IDENTITIES_ANSWER
    uint32      num_keys
...
```

#### <a name="apidoc.element.ssh2.Channel.prototype.eof"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>eof ()](#apidoc.element.ssh2.Channel.prototype.eof)
- description and source-code
```javascript
eof = function () {
  var ret = true;
  var outgoing = this.outgoing;

  if (outgoing.state === 'open') {
    outgoing.state = 'eof';
    ret = this._client._sshstream.channelEOF(outgoing.id);
  }

  return ret;
}
```
- example usage
```shell
...

this._chunk = undefined;
this._chunkcb = undefined;
this._chunkErr = undefined;
this._chunkcbErr = undefined;

function onFinish() {
  self.eof();
  if (server || (!server && !self.allowHalfOpen))
    self.close();
  self.writable = false;
}
this.on('finish', onFinish)
    .on('prefinish', onFinish); // for node v0.11+
function onEnd() {
...
```

#### <a name="apidoc.element.ssh2.Channel.prototype.exit"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>exit (name, coreDumped, msg)](#apidoc.element.ssh2.Channel.prototype.exit)
- description and source-code
```javascript
exit = function (name, coreDumped, msg) {
  if (!this.server)
    throw new Error('Server-only method called in client mode');

  if (this.type === 'session'
      && this.writable
      && this.outgoing.state === 'open') {
    if (typeof name === 'number')
      return this._client._sshstream.exitStatus(this.outgoing.id, name);
    else {
      return this._client._sshstream.exitSignal(this.outgoing.id,
                                                name,
                                                coreDumped,
                                                msg);
    }
  }

  return true;
}
```
- example usage
```shell
...
    client.on('session', function(accept, reject) {
      var session = accept();
      session.once('exec', function(accept, reject, info) {
        console.log('Client wants to execute: ' + inspect(info.command));
        var stream = accept();
        stream.stderr.write('Oh no, the dreaded errors!\n');
        stream.write('Just kidding about the errors!\n');
        stream.exit(0);
        stream.end();
      });
    });
  }).on('end', function() {
    console.log('Client disconnected');
  });
}).listen(0, '127.0.0.1', function() {
...
```

#### <a name="apidoc.element.ssh2.Channel.prototype.setWindow"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>setWindow (rows, cols, height, width)](#apidoc.element.ssh2.Channel.prototype.setWindow)
- description and source-code
```javascript
setWindow = function (rows, cols, height, width) {
  if (this.server)
    throw new Error('Client-only method called in server mode');

  if (this.type === 'session'
      && (this.subtype === 'shell' || this.subtype === 'exec')
      && this.writable
      && this.outgoing.state === 'open') {
    return this._client._sshstream.windowChange(this.outgoing.id,
                                                rows,
                                                cols,
                                                height,
                                                width);
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Channel.prototype.signal"></a>[function <span class="apidocSignatureSpan">ssh2.Channel.prototype.</span>signal (signalName)](#apidoc.element.ssh2.Channel.prototype.signal)
- description and source-code
```javascript
signal = function (signalName) {
  if (this.server)
    throw new Error('Client-only method called in server mode');

  if (this.type === 'session'
      && this.writable
      && this.outgoing.state === 'open')
    return this._client._sshstream.signal(this.outgoing.id, signalName);

  return true;
}
```
- example usage
```shell
...
Channel.prototype.signal = function(signalName) {
if (this.server)
  throw new Error('Client-only method called in server mode');

if (this.type === 'session'
    && this.writable
    && this.outgoing.state === 'open')
  return this._client._sshstream.signal(this.outgoing.id, signalName);

return true;
};
Channel.prototype.exit = function(name, coreDumped, msg) {
if (!this.server)
  throw new Error('Server-only method called in client mode');
...
```



# <a name="apidoc.module.ssh2.SFTPWrapper"></a>[module ssh2.SFTPWrapper](#apidoc.module.ssh2.SFTPWrapper)

#### <a name="apidoc.element.ssh2.SFTPWrapper.SFTPWrapper"></a>[function <span class="apidocSignatureSpan">ssh2.</span>SFTPWrapper (stream)](#apidoc.element.ssh2.SFTPWrapper.SFTPWrapper)
- description and source-code
```javascript
function SFTPWrapper(stream) {
  var self = this;

  EventEmitter.call(this);

  this._stream = stream;

  stream.on('error', function(err) {
    self.emit('error', err);
  }).on('end', function() {
    self.emit('end');
  }).on('close', function() {
    self.emit('close');
  }).on('continue', function() {
    self.emit('continue');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.super_"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.</span>super_ ()](#apidoc.element.ssh2.SFTPWrapper.super_)
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



# <a name="apidoc.module.ssh2.SFTPWrapper.prototype"></a>[module ssh2.SFTPWrapper.prototype](#apidoc.module.ssh2.SFTPWrapper.prototype)

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.appendFile"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>appendFile (path, data, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.appendFile)
- description and source-code
```javascript
appendFile = function (path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.readFile = function(path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
};
SFTPWrapper.prototype.writeFile = function(path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
};
SFTPWrapper.prototype.appendFile = function(path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
};
SFTPWrapper.prototype.exists = function(path, cb) {
  return this._stream.exists(path, cb);
};
SFTPWrapper.prototype.unlink = function(filename, cb) {
  return this._stream.unlink(filename, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.chmod"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>chmod (path, mode, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.chmod)
- description and source-code
```javascript
chmod = function (path, mode, cb) {
  return this._stream.chmod(path, mode, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.chown = function(path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
};
SFTPWrapper.prototype.fchmod = function(handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
};
SFTPWrapper.prototype.chmod = function(path, mode, cb) {
  return this._stream.chmod(path, mode, cb);
};
SFTPWrapper.prototype.readlink = function(path, cb) {
  return this._stream.readlink(path, cb);
};
SFTPWrapper.prototype.symlink = function(targetPath, linkPath, cb) {
  return this._stream.symlink(targetPath, linkPath, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.chown"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>chown (path, uid, gid, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.chown)
- description and source-code
```javascript
chown = function (path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.utimes = function(path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
};
SFTPWrapper.prototype.fchown = function(handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
};
SFTPWrapper.prototype.chown = function(path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
};
SFTPWrapper.prototype.fchmod = function(handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
};
SFTPWrapper.prototype.chmod = function(path, mode, cb) {
  return this._stream.chmod(path, mode, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.close"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>close (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.close)
- description and source-code
```javascript
close = function (handle, cb) {
  return this._stream.close(handle, cb);
}
```
- example usage
```shell
...
  self.push(null);
if (server && self.stderr.writable)
  self.stderr.end();
else if (!server && self.stderr.readable)
  self.stderr.push(null);

if (outgoing.state === 'open' || outgoing.state === 'eof')
  self.close();
if (outgoing.state === 'closing')
  outgoing.state = 'closed';

delete channels[incomingId];

var state = self._writableState;
client._sock.removeListener('drain', ondrain);
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.createReadStream"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>createReadStream (path, options)](#apidoc.element.ssh2.SFTPWrapper.prototype.createReadStream)
- description and source-code
```javascript
createReadStream = function (path, options) {
  return this._stream.createReadStream(path, options);
}
```
- example usage
```shell
...

// stream-related methods to pass on
SFTPWrapper.prototype.end = function() {
  return this._stream.end();
};
// SFTPStream client methods
SFTPWrapper.prototype.createReadStream = function(path, options) {
  return this._stream.createReadStream(path, options);
};
SFTPWrapper.prototype.createWriteStream = function(path, options) {
  return this._stream.createWriteStream(path, options);
};
SFTPWrapper.prototype.open = function(path, flags, attrs, cb) {
  return this._stream.open(path, flags, attrs, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.createWriteStream"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>createWriteStream (path, options)](#apidoc.element.ssh2.SFTPWrapper.prototype.createWriteStream)
- description and source-code
```javascript
createWriteStream = function (path, options) {
  return this._stream.createWriteStream(path, options);
}
```
- example usage
```shell
...
  return this._stream.end();
};
// SFTPStream client methods
SFTPWrapper.prototype.createReadStream = function(path, options) {
  return this._stream.createReadStream(path, options);
};
SFTPWrapper.prototype.createWriteStream = function(path, options) {
  return this._stream.createWriteStream(path, options);
};
SFTPWrapper.prototype.open = function(path, flags, attrs, cb) {
  return this._stream.open(path, flags, attrs, cb);
};
SFTPWrapper.prototype.close = function(handle, cb) {
  return this._stream.close(handle, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.end"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>end ()](#apidoc.element.ssh2.SFTPWrapper.prototype.end)
- description and source-code
```javascript
end = function () {
  return this._stream.end();
}
```
- example usage
```shell
...
var conn = new Client();
conn.on('ready', function() {
  console.log('Client :: ready');
  conn.exec('uptime', function(err, stream) {
    if (err) throw err;
    stream.on('close', function(code, signal) {
      console.log('Stream :: close :: code: ' + code + ', signal: ' + signal);
      conn.end();
    }).on('data', function(data) {
      console.log('STDOUT: ' + data);
    }).stderr.on('data', function(data) {
      console.log('STDERR: ' + data);
    });
  });
}).connect({
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.exists"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>exists (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.exists)
- description and source-code
```javascript
exists = function (path, cb) {
  return this._stream.exists(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.writeFile = function(path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
};
SFTPWrapper.prototype.appendFile = function(path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
};
SFTPWrapper.prototype.exists = function(path, cb) {
  return this._stream.exists(path, cb);
};
SFTPWrapper.prototype.unlink = function(filename, cb) {
  return this._stream.unlink(filename, cb);
};
SFTPWrapper.prototype.rename = function(oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fstatvfs"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_fstatvfs (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fstatvfs)
- description and source-code
```javascript
ext_openssh_fstatvfs = function (handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.ext_openssh_rename = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_statvfs = function(path, cb) {
  return this._stream.ext_openssh_statvfs(path, cb);
};
SFTPWrapper.prototype.ext_openssh_fstatvfs = function(handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
};
SFTPWrapper.prototype.ext_openssh_hardlink = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_hardlink(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_fsync = function(handle, cb) {
  return this._stream.ext_openssh_fsync(handle, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fsync"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_fsync (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_fsync)
- description and source-code
```javascript
ext_openssh_fsync = function (handle, cb) {
  return this._stream.ext_openssh_fsync(handle, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.ext_openssh_fstatvfs = function(handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
};
SFTPWrapper.prototype.ext_openssh_hardlink = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_hardlink(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_fsync = function(handle, cb) {
  return this._stream.ext_openssh_fsync(handle, cb);
};

module.exports = SFTPWrapper;
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_hardlink"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_hardlink (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_hardlink)
- description and source-code
```javascript
ext_openssh_hardlink = function (oldPath, newPath, cb) {
  return this._stream.ext_openssh_hardlink(oldPath, newPath, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.ext_openssh_statvfs = function(path, cb) {
  return this._stream.ext_openssh_statvfs(path, cb);
};
SFTPWrapper.prototype.ext_openssh_fstatvfs = function(handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
};
SFTPWrapper.prototype.ext_openssh_hardlink = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_hardlink(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_fsync = function(handle, cb) {
  return this._stream.ext_openssh_fsync(handle, cb);
};

module.exports = SFTPWrapper;
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_rename"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_rename (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_rename)
- description and source-code
```javascript
ext_openssh_rename = function (oldPath, newPath, cb) {
  return this._stream.ext_openssh_rename(oldPath, newPath, cb);
}
```
- example usage
```shell
...
  return this._stream.symlink(targetPath, linkPath, cb);
};
SFTPWrapper.prototype.realpath = function(path, cb) {
  return this._stream.realpath(path, cb);
};
// extended requests
SFTPWrapper.prototype.ext_openssh_rename = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_statvfs = function(path, cb) {
  return this._stream.ext_openssh_statvfs(path, cb);
};
SFTPWrapper.prototype.ext_openssh_fstatvfs = function(handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_statvfs"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>ext_openssh_statvfs (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.ext_openssh_statvfs)
- description and source-code
```javascript
ext_openssh_statvfs = function (path, cb) {
  return this._stream.ext_openssh_statvfs(path, cb);
}
```
- example usage
```shell
...
  return this._stream.realpath(path, cb);
};
// extended requests
SFTPWrapper.prototype.ext_openssh_rename = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_statvfs = function(path, cb) {
  return this._stream.ext_openssh_statvfs(path, cb);
};
SFTPWrapper.prototype.ext_openssh_fstatvfs = function(handle, cb) {
  return this._stream.ext_openssh_fstatvfs(handle, cb);
};
SFTPWrapper.prototype.ext_openssh_hardlink = function(oldPath, newPath, cb) {
  return this._stream.ext_openssh_hardlink(oldPath, newPath, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fastGet"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fastGet (remotePath, localPath, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fastGet)
- description and source-code
```javascript
fastGet = function (remotePath, localPath, opts, cb) {
  return this._stream.fastGet(remotePath, localPath, opts, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.read = function(handle, buf, off, len, position, cb) {
  return this._stream.readData(handle, buf, off, len, position, cb);
};
SFTPWrapper.prototype.write = function(handle, buf, off, len, position, cb) {
  return this._stream.writeData(handle, buf, off, len, position, cb);
};
SFTPWrapper.prototype.fastGet = function(remotePath, localPath, opts, cb) {
  return this._stream.fastGet(remotePath, localPath, opts, cb);
};
SFTPWrapper.prototype.fastPut = function(localPath, remotePath, opts, cb) {
  return this._stream.fastPut(localPath, remotePath, opts, cb);
};
SFTPWrapper.prototype.readFile = function(path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fastPut"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fastPut (localPath, remotePath, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fastPut)
- description and source-code
```javascript
fastPut = function (localPath, remotePath, opts, cb) {
  return this._stream.fastPut(localPath, remotePath, opts, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.write = function(handle, buf, off, len, position, cb) {
  return this._stream.writeData(handle, buf, off, len, position, cb);
};
SFTPWrapper.prototype.fastGet = function(remotePath, localPath, opts, cb) {
  return this._stream.fastGet(remotePath, localPath, opts, cb);
};
SFTPWrapper.prototype.fastPut = function(localPath, remotePath, opts, cb) {
  return this._stream.fastPut(localPath, remotePath, opts, cb);
};
SFTPWrapper.prototype.readFile = function(path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
};
SFTPWrapper.prototype.writeFile = function(path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fchmod"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fchmod (handle, mode, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fchmod)
- description and source-code
```javascript
fchmod = function (handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fchown = function(handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
};
SFTPWrapper.prototype.chown = function(path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
};
SFTPWrapper.prototype.fchmod = function(handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
};
SFTPWrapper.prototype.chmod = function(path, mode, cb) {
  return this._stream.chmod(path, mode, cb);
};
SFTPWrapper.prototype.readlink = function(path, cb) {
  return this._stream.readlink(path, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fchown"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fchown (handle, uid, gid, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fchown)
- description and source-code
```javascript
fchown = function (handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.futimes = function(handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
};
SFTPWrapper.prototype.utimes = function(path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
};
SFTPWrapper.prototype.fchown = function(handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
};
SFTPWrapper.prototype.chown = function(path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
};
SFTPWrapper.prototype.fchmod = function(handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fsetstat"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fsetstat (handle, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fsetstat)
- description and source-code
```javascript
fsetstat = function (handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.opendir = function(path, cb) {
  return this._stream.opendir(path, cb);
};
SFTPWrapper.prototype.setstat = function(path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
};
SFTPWrapper.prototype.fsetstat = function(handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
};
SFTPWrapper.prototype.futimes = function(handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
};
SFTPWrapper.prototype.utimes = function(path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.fstat"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>fstat (handle, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.fstat)
- description and source-code
```javascript
fstat = function (handle, cb) {
  return this._stream.fstat(handle, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.rmdir = function(path, cb) {
  return this._stream.rmdir(path, cb);
};
SFTPWrapper.prototype.readdir = function(where, opts, cb) {
  return this._stream.readdir(where, opts, cb);
};
SFTPWrapper.prototype.fstat = function(handle, cb) {
  return this._stream.fstat(handle, cb);
};
SFTPWrapper.prototype.stat = function(path, cb) {
  return this._stream.stat(path, cb);
};
SFTPWrapper.prototype.lstat = function(path, cb) {
  return this._stream.lstat(path, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.futimes"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>futimes (handle, atime, mtime, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.futimes)
- description and source-code
```javascript
futimes = function (handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.setstat = function(path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
};
SFTPWrapper.prototype.fsetstat = function(handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
};
SFTPWrapper.prototype.futimes = function(handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
};
SFTPWrapper.prototype.utimes = function(path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
};
SFTPWrapper.prototype.fchown = function(handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.lstat"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>lstat (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.lstat)
- description and source-code
```javascript
lstat = function (path, cb) {
  return this._stream.lstat(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fstat = function(handle, cb) {
  return this._stream.fstat(handle, cb);
};
SFTPWrapper.prototype.stat = function(path, cb) {
  return this._stream.stat(path, cb);
};
SFTPWrapper.prototype.lstat = function(path, cb) {
  return this._stream.lstat(path, cb);
};
SFTPWrapper.prototype.opendir = function(path, cb) {
  return this._stream.opendir(path, cb);
};
SFTPWrapper.prototype.setstat = function(path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.mkdir"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>mkdir (path, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.mkdir)
- description and source-code
```javascript
mkdir = function (path, attrs, cb) {
  return this._stream.mkdir(path, attrs, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.unlink = function(filename, cb) {
  return this._stream.unlink(filename, cb);
};
SFTPWrapper.prototype.rename = function(oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.mkdir = function(path, attrs, cb) {
  return this._stream.mkdir(path, attrs, cb);
};
SFTPWrapper.prototype.rmdir = function(path, cb) {
  return this._stream.rmdir(path, cb);
};
SFTPWrapper.prototype.readdir = function(where, opts, cb) {
  return this._stream.readdir(where, opts, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.open"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>open (path, flags, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.open)
- description and source-code
```javascript
open = function (path, flags, attrs, cb) {
  return this._stream.open(path, flags, attrs, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.createReadStream = function(path, options) {
  return this._stream.createReadStream(path, options);
};
SFTPWrapper.prototype.createWriteStream = function(path, options) {
  return this._stream.createWriteStream(path, options);
};
SFTPWrapper.prototype.open = function(path, flags, attrs, cb) {
  return this._stream.open(path, flags, attrs, cb);
};
SFTPWrapper.prototype.close = function(handle, cb) {
  return this._stream.close(handle, cb);
};
SFTPWrapper.prototype.read = function(handle, buf, off, len, position, cb) {
  return this._stream.readData(handle, buf, off, len, position, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.opendir"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>opendir (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.opendir)
- description and source-code
```javascript
opendir = function (path, cb) {
  return this._stream.opendir(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.stat = function(path, cb) {
  return this._stream.stat(path, cb);
};
SFTPWrapper.prototype.lstat = function(path, cb) {
  return this._stream.lstat(path, cb);
};
SFTPWrapper.prototype.opendir = function(path, cb) {
  return this._stream.opendir(path, cb);
};
SFTPWrapper.prototype.setstat = function(path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
};
SFTPWrapper.prototype.fsetstat = function(handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.read"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>read (handle, buf, off, len, position, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.read)
- description and source-code
```javascript
read = function (handle, buf, off, len, position, cb) {
  return this._stream.readData(handle, buf, off, len, position, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.readFile"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readFile (path, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.readFile)
- description and source-code
```javascript
readFile = function (path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fastGet = function(remotePath, localPath, opts, cb) {
  return this._stream.fastGet(remotePath, localPath, opts, cb);
};
SFTPWrapper.prototype.fastPut = function(localPath, remotePath, opts, cb) {
  return this._stream.fastPut(localPath, remotePath, opts, cb);
};
SFTPWrapper.prototype.readFile = function(path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
};
SFTPWrapper.prototype.writeFile = function(path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
};
SFTPWrapper.prototype.appendFile = function(path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.readdir"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readdir (where, opts, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.readdir)
- description and source-code
```javascript
readdir = function (where, opts, cb) {
  return this._stream.readdir(where, opts, cb);
}
```
- example usage
```shell
...
var Client = require('ssh2').Client;

var conn = new Client();
conn.on('ready', function() {
console.log('Client :: ready');
conn.sftp(function(err, sftp) {
  if (err) throw err;
  sftp.readdir('foo', function(err, list) {
    if (err) throw err;
    console.dir(list);
    conn.end();
  });
});
}).connect({
host: '192.168.100.100',
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.readlink"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>readlink (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.readlink)
- description and source-code
```javascript
readlink = function (path, cb) {
  return this._stream.readlink(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fchmod = function(handle, mode, cb) {
  return this._stream.fchmod(handle, mode, cb);
};
SFTPWrapper.prototype.chmod = function(path, mode, cb) {
  return this._stream.chmod(path, mode, cb);
};
SFTPWrapper.prototype.readlink = function(path, cb) {
  return this._stream.readlink(path, cb);
};
SFTPWrapper.prototype.symlink = function(targetPath, linkPath, cb) {
  return this._stream.symlink(targetPath, linkPath, cb);
};
SFTPWrapper.prototype.realpath = function(path, cb) {
  return this._stream.realpath(path, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.realpath"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>realpath (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.realpath)
- description and source-code
```javascript
realpath = function (path, cb) {
  return this._stream.realpath(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.readlink = function(path, cb) {
return this._stream.readlink(path, cb);
};
SFTPWrapper.prototype.symlink = function(targetPath, linkPath, cb) {
return this._stream.symlink(targetPath, linkPath, cb);
};
SFTPWrapper.prototype.realpath = function(path, cb) {
return this._stream.realpath(path, cb);
};
// extended requests
SFTPWrapper.prototype.ext_openssh_rename = function(oldPath, newPath, cb) {
return this._stream.ext_openssh_rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.ext_openssh_statvfs = function(path, cb) {
return this._stream.ext_openssh_statvfs(path, cb);
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.rename"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>rename (oldPath, newPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.rename)
- description and source-code
```javascript
rename = function (oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.exists = function(path, cb) {
  return this._stream.exists(path, cb);
};
SFTPWrapper.prototype.unlink = function(filename, cb) {
  return this._stream.unlink(filename, cb);
};
SFTPWrapper.prototype.rename = function(oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.mkdir = function(path, attrs, cb) {
  return this._stream.mkdir(path, attrs, cb);
};
SFTPWrapper.prototype.rmdir = function(path, cb) {
  return this._stream.rmdir(path, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.rmdir"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>rmdir (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.rmdir)
- description and source-code
```javascript
rmdir = function (path, cb) {
  return this._stream.rmdir(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.rename = function(oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.mkdir = function(path, attrs, cb) {
  return this._stream.mkdir(path, attrs, cb);
};
SFTPWrapper.prototype.rmdir = function(path, cb) {
  return this._stream.rmdir(path, cb);
};
SFTPWrapper.prototype.readdir = function(where, opts, cb) {
  return this._stream.readdir(where, opts, cb);
};
SFTPWrapper.prototype.fstat = function(handle, cb) {
  return this._stream.fstat(handle, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.setstat"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>setstat (path, attrs, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.setstat)
- description and source-code
```javascript
setstat = function (path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.lstat = function(path, cb) {
  return this._stream.lstat(path, cb);
};
SFTPWrapper.prototype.opendir = function(path, cb) {
  return this._stream.opendir(path, cb);
};
SFTPWrapper.prototype.setstat = function(path, attrs, cb) {
  return this._stream.setstat(path, attrs, cb);
};
SFTPWrapper.prototype.fsetstat = function(handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
};
SFTPWrapper.prototype.futimes = function(handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.stat"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>stat (path, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.stat)
- description and source-code
```javascript
stat = function (path, cb) {
  return this._stream.stat(path, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.readdir = function(where, opts, cb) {
  return this._stream.readdir(where, opts, cb);
};
SFTPWrapper.prototype.fstat = function(handle, cb) {
  return this._stream.fstat(handle, cb);
};
SFTPWrapper.prototype.stat = function(path, cb) {
  return this._stream.stat(path, cb);
};
SFTPWrapper.prototype.lstat = function(path, cb) {
  return this._stream.lstat(path, cb);
};
SFTPWrapper.prototype.opendir = function(path, cb) {
  return this._stream.opendir(path, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.symlink"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>symlink (targetPath, linkPath, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.symlink)
- description and source-code
```javascript
symlink = function (targetPath, linkPath, cb) {
  return this._stream.symlink(targetPath, linkPath, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.chmod = function(path, mode, cb) {
return this._stream.chmod(path, mode, cb);
};
SFTPWrapper.prototype.readlink = function(path, cb) {
return this._stream.readlink(path, cb);
};
SFTPWrapper.prototype.symlink = function(targetPath, linkPath, cb) {
return this._stream.symlink(targetPath, linkPath, cb);
};
SFTPWrapper.prototype.realpath = function(path, cb) {
return this._stream.realpath(path, cb);
};
// extended requests
SFTPWrapper.prototype.ext_openssh_rename = function(oldPath, newPath, cb) {
return this._stream.ext_openssh_rename(oldPath, newPath, cb);
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.unlink"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>unlink (filename, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.unlink)
- description and source-code
```javascript
unlink = function (filename, cb) {
  return this._stream.unlink(filename, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.appendFile = function(path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
};
SFTPWrapper.prototype.exists = function(path, cb) {
  return this._stream.exists(path, cb);
};
SFTPWrapper.prototype.unlink = function(filename, cb) {
  return this._stream.unlink(filename, cb);
};
SFTPWrapper.prototype.rename = function(oldPath, newPath, cb) {
  return this._stream.rename(oldPath, newPath, cb);
};
SFTPWrapper.prototype.mkdir = function(path, attrs, cb) {
  return this._stream.mkdir(path, attrs, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.utimes"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>utimes (path, atime, mtime, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.utimes)
- description and source-code
```javascript
utimes = function (path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fsetstat = function(handle, attrs, cb) {
  return this._stream.fsetstat(handle, attrs, cb);
};
SFTPWrapper.prototype.futimes = function(handle, atime, mtime, cb) {
  return this._stream.futimes(handle, atime, mtime, cb);
};
SFTPWrapper.prototype.utimes = function(path, atime, mtime, cb) {
  return this._stream.utimes(path, atime, mtime, cb);
};
SFTPWrapper.prototype.fchown = function(handle, uid, gid, cb) {
  return this._stream.fchown(handle, uid, gid, cb);
};
SFTPWrapper.prototype.chown = function(path, uid, gid, cb) {
  return this._stream.chown(path, uid, gid, cb);
};
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.write"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>write (handle, buf, off, len, position, cb)](#apidoc.element.ssh2.SFTPWrapper.prototype.write)
- description and source-code
```javascript
write = function (handle, buf, off, len, position, cb) {
  return this._stream.writeData(handle, buf, off, len, position, cb);
}
```
- example usage
```shell
...

conn.on('ready', function() {
  console.log('Client :: ready');
  conn.subsys('netconf', function(err, stream) {
    if (err) throw err;
    stream.on('data', function(data) {
      console.log(data);
    }).write(xmlhello);
  });
}).connect({
  host: '1.2.3.4',
  port: 22,
  username: 'blargh',
  password: 'honk'
});
...
```

#### <a name="apidoc.element.ssh2.SFTPWrapper.prototype.writeFile"></a>[function <span class="apidocSignatureSpan">ssh2.SFTPWrapper.prototype.</span>writeFile (path, data, options, callback_)](#apidoc.element.ssh2.SFTPWrapper.prototype.writeFile)
- description and source-code
```javascript
writeFile = function (path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
}
```
- example usage
```shell
...
SFTPWrapper.prototype.fastPut = function(localPath, remotePath, opts, cb) {
  return this._stream.fastPut(localPath, remotePath, opts, cb);
};
SFTPWrapper.prototype.readFile = function(path, options, callback_) {
  return this._stream.readFile(path, options, callback_);
};
SFTPWrapper.prototype.writeFile = function(path, data, options, callback_) {
  return this._stream.writeFile(path, data, options, callback_);
};
SFTPWrapper.prototype.appendFile = function(path, data, options, callback_) {
  return this._stream.appendFile(path, data, options, callback_);
};
SFTPWrapper.prototype.exists = function(path, cb) {
  return this._stream.exists(path, cb);
};
...
```



# <a name="apidoc.module.ssh2.Server"></a>[module ssh2.Server](#apidoc.module.ssh2.Server)

#### <a name="apidoc.element.ssh2.Server.Server"></a>[function <span class="apidocSignatureSpan">ssh2.</span>Server (cfg, listener)](#apidoc.element.ssh2.Server.Server)
- description and source-code
```javascript
function Server(cfg, listener) {
  if (!(this instanceof Server))
    return new Server(cfg, listener);

  var hostKeys = {
    'ssh-rsa': null,
    'ssh-dss': null,
    'ecdsa-sha2-nistp256': null,
    'ecdsa-sha2-nistp384': null,
    'ecdsa-sha2-nistp521': null
  };

  var hostKeys_ = cfg.hostKeys;
  if (!Array.isArray(hostKeys_))
    throw new Error('hostKeys must be an array');

  var i;
  for (i = 0; i < hostKeys_.length; ++i) {
    var privateKey;
    if (Buffer.isBuffer(hostKeys_[i]) || typeof hostKeys_[i] === 'string')
      privateKey = parseKey(hostKeys_[i]);
    else
      privateKey = parseKey(hostKeys_[i].key);
    if (privateKey instanceof Error)
      throw new Error('Cannot parse privateKey: ' + privateKey.message);
    if (!privateKey.private)
      throw new Error('privateKey value contains an invalid private key');
    if (hostKeys[privateKey.fulltype])
      continue;
    if (privateKey.encryption) {
      if (typeof hostKeys_[i].passphrase !== 'string')
        throw new Error('Missing passphrase for encrypted private key');
      decryptKey(privateKey, hostKeys_[i].passphrase);
    }
    hostKeys[privateKey.fulltype] = {
      privateKey: privateKey,
      publicKey: genPublicKey(privateKey)
    };
  }

  var algorithms = {
    kex: undefined,
    kexBuf: undefined,
    cipher: undefined,
    cipherBuf: undefined,
    serverHostKey: undefined,
    serverHostKeyBuf: undefined,
    hmac: undefined,
    hmacBuf: undefined,
    compress: undefined,
    compressBuf: undefined
  };
  if (typeof cfg.algorithms === 'object' && cfg.algorithms !== null) {
    var algosSupported;
    var algoList;

    algoList = cfg.algorithms.kex;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_KEX;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported key exchange algorithm: ' + algoList[i]);
      }
      algorithms.kex = algoList;
    }

    algoList = cfg.algorithms.cipher;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_CIPHER;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported cipher algorithm: ' + algoList[i]);
      }
      algorithms.cipher = algoList;
    }

    algoList = cfg.algorithms.serverHostKey;
    var copied = false;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_SERVER_HOST_KEY;
      for (i = algoList.length - 1; i >= 0; --i) {
        if (algosSupported.indexOf(algoList[i]) === -1) {
          throw new Error('Unsupported server host key algorithm: '
                           + algoList[i]);
        }
        if (!hostKeys[algoList[i]]) {
          // Silently discard for now
          if (!copied) {
            algoList = algoList.slice();
            copied = true;
          }
          algoList.splice(i, 1);
        }
      }
      if (algoList.length > 0)
        algorithms.serverHostKey = algoList;
    }

    algoList = cfg.algorithms.hmac;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_HMAC;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported HMAC algorithm: ' + algoList[i]);
      }
      algorithms.hmac = algoList;
    }

    algoList = cfg.algorithms.compress;
    if (Array.isArray(algoList) && algoList.length > 0) {
      algosSupported = ALGORITHMS.SUPPORTED_COMPRESS;
      for (i = 0; i < algoList.length; ++i) {
        if (algosSupported.indexOf(algoList[i]) === -1)
          throw new Error('Unsupported compression algorithm: ' + algoList[i]);
      }
      algorithms.compress = algoList;
    }
  }

  // Make sure we at least have some kind of valid list of support key
  // formats
  if (algorithms.serverHostKey === undefined) {
    var hostKeyAlgos = Object.keys(hostKeys);
    for (i = hostKeyAlgos.length - 1; i ...
```
- example usage
```shell
...

var buffersEqual = require('buffer-equal-constant-time');
var ssh2 = require('ssh2');
var utils = ssh2.utils;

var pubKey = utils.genPublicKey(utils.parseKey(fs.readFileSync('user.pub')));

new ssh2.Server({
hostKeys: [fs.readFileSync('host.key')]
}, function(client) {
console.log('Client connected!');

client.on('authentication', function(ctx) {
  if (ctx.method === 'password'
      && ctx.username === 'foo'
...
```

#### <a name="apidoc.element.ssh2.Server.createServer"></a>[function <span class="apidocSignatureSpan">ssh2.Server.</span>createServer (cfg, listener)](#apidoc.element.ssh2.Server.createServer)
- description and source-code
```javascript
createServer = function (cfg, listener) {
  return new Server(cfg, listener);
}
```
- example usage
```shell
...
var ssh_config = {
host: '192.168.100.1',
port: 22,
username: 'nodejs',
password: 'rules'
};

socks.createServer(function(info, accept, deny) {
// NOTE: you could just use one ssh2 client connection for all forwards, but
// you could run into server-imposed limits if you have too many forwards open
// at any given time
var conn = new Client();
conn.on('ready', function() {
  conn.forwardOut(info.srcAddr,
                  info.srcPort,
...
```

#### <a name="apidoc.element.ssh2.Server.super_"></a>[function <span class="apidocSignatureSpan">ssh2.Server.</span>super_ ()](#apidoc.element.ssh2.Server.super_)
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



# <a name="apidoc.module.ssh2.Server.prototype"></a>[module ssh2.Server.prototype](#apidoc.module.ssh2.Server.prototype)

#### <a name="apidoc.element.ssh2.Server.prototype.address"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>address ()](#apidoc.element.ssh2.Server.prototype.address)
- description and source-code
```javascript
address = function () {
  return this._srv.address();
}
```
- example usage
```shell
...
        stream.end();
      });
    });
  }).on('end', function() {
    console.log('Client disconnected');
  });
}).listen(0, '127.0.0.1', function() {
  console.log('Listening on port ' + this.address().port);
});
'''

* SFTP only server:

'''javascript
var fs = require('fs');
...
```

#### <a name="apidoc.element.ssh2.Server.prototype.close"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>close (cb)](#apidoc.element.ssh2.Server.prototype.close)
- description and source-code
```javascript
close = function (cb) {
  this._srv.close(cb);
  return this;
}
```
- example usage
```shell
...
  self.push(null);
if (server && self.stderr.writable)
  self.stderr.end();
else if (!server && self.stderr.readable)
  self.stderr.push(null);

if (outgoing.state === 'open' || outgoing.state === 'eof')
  self.close();
if (outgoing.state === 'closing')
  outgoing.state = 'closed';

delete channels[incomingId];

var state = self._writableState;
client._sock.removeListener('drain', ondrain);
...
```

#### <a name="apidoc.element.ssh2.Server.prototype.getConnections"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>getConnections (cb)](#apidoc.element.ssh2.Server.prototype.getConnections)
- description and source-code
```javascript
getConnections = function (cb) {
  this._srv.getConnections(cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Server.prototype.listen"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>listen ()](#apidoc.element.ssh2.Server.prototype.listen)
- description and source-code
```javascript
listen = function () {
  this._srv.listen.apply(this._srv, arguments);
  return this;
}
```
- example usage
```shell
...
        });
      } else
        conn.end();
    });
  }).on('error', function(err) {
    deny();
  }).connect(ssh_config);
}).listen(1080, 'localhost', function() {
  console.log('SOCKSv5 proxy server started on port 1080');
}).useAuth(socks.auth.None());

// test with cURL:
//   curl -i --socks5 localhost:1080 google.com
'''
...
```

#### <a name="apidoc.element.ssh2.Server.prototype.ref"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>ref ()](#apidoc.element.ssh2.Server.prototype.ref)
- description and source-code
```javascript
ref = function () {
  this._srv.ref();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.Server.prototype.unref"></a>[function <span class="apidocSignatureSpan">ssh2.Server.prototype.</span>unref ()](#apidoc.element.ssh2.Server.prototype.unref)
- description and source-code
```javascript
unref = function () {
  this._srv.unref();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ssh2.keepalivemgr"></a>[module ssh2.keepalivemgr](#apidoc.module.ssh2.keepalivemgr)

#### <a name="apidoc.element.ssh2.keepalivemgr.keepalivemgr"></a>[function <span class="apidocSignatureSpan">ssh2.</span>keepalivemgr (interval, streamInterval, kaCountMax)](#apidoc.element.ssh2.keepalivemgr.keepalivemgr)
- description and source-code
```javascript
function Manager(interval, streamInterval, kaCountMax) {
  var streams = this._streams = [];
  this._timer = undefined;
  this._timerInterval = interval;
  this._timerfn = function() {
    var now = Date.now();
    for (var i = 0, len = streams.length, s, last; i < len; ++i) {
      s = streams[i];
      last = s._kalast;
      if (last && (now - last) >= streamInterval) {
        if (++s._kacnt > kaCountMax) {
          var err = new Error('Keepalive timeout');
          err.level = 'client-timeout';
          s.emit('error', err);
          s.disconnect();
          spliceOne(streams, i);
          --i;
          len = streams.length;
        } else {
          s._kalast = now;
          // XXX: if the server ever starts sending real global requests to the
          //      client, we will need to add a dummy callback here to keep the
          //      correct reply order
          s.ping();
        }
      }
    }
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ssh2.keepalivemgr.prototype"></a>[module ssh2.keepalivemgr.prototype](#apidoc.module.ssh2.keepalivemgr.prototype)

#### <a name="apidoc.element.ssh2.keepalivemgr.prototype.add"></a>[function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>add (stream)](#apidoc.element.ssh2.keepalivemgr.prototype.add)
- description and source-code
```javascript
add = function (stream) {
  var streams = this._streams,
      self = this;

  stream.once('end', function() {
    self.remove(stream);
  }).on('packet', resetKA);

  streams[streams.length] = stream;

  resetKA();

  if (!this._timer)
    this.start();

  function resetKA() {
    stream._kalast = Date.now();
    stream._kacnt = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.keepalivemgr.prototype.remove"></a>[function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>remove (stream)](#apidoc.element.ssh2.keepalivemgr.prototype.remove)
- description and source-code
```javascript
remove = function (stream) {
  var streams = this._streams,
      index = streams.indexOf(stream);
  if (index > -1)
    spliceOne(streams, index);
  if (!streams.length)
    this.stop();
}
```
- example usage
```shell
...
};

Manager.prototype.add = function(stream) {
var streams = this._streams,
    self = this;

stream.once('end', function() {
  self.remove(stream);
}).on('packet', resetKA);

streams[streams.length] = stream;

resetKA();

if (!this._timer)
...
```

#### <a name="apidoc.element.ssh2.keepalivemgr.prototype.start"></a>[function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>start ()](#apidoc.element.ssh2.keepalivemgr.prototype.start)
- description and source-code
```javascript
start = function () {
  if (this._timer)
    this.stop();
  this._timer = setInterval(this._timerfn, this._timerInterval);
}
```
- example usage
```shell
...
  }).on('packet', resetKA);

  streams[streams.length] = stream;

  resetKA();

  if (!this._timer)
    this.start();

  function resetKA() {
    stream._kalast = Date.now();
    stream._kacnt = 0;
  }
};
...
```

#### <a name="apidoc.element.ssh2.keepalivemgr.prototype.stop"></a>[function <span class="apidocSignatureSpan">ssh2.keepalivemgr.prototype.</span>stop ()](#apidoc.element.ssh2.keepalivemgr.prototype.stop)
- description and source-code
```javascript
stop = function () {
  if (this._timer) {
    clearInterval(this._timer);
    this._timer = undefined;
  }
}
```
- example usage
```shell
...
    }
  }
};
}

Manager.prototype.start = function() {
if (this._timer)
  this.stop();
this._timer = setInterval(this._timerfn, this._timerInterval);
};

Manager.prototype.stop = function() {
if (this._timer) {
  clearInterval(this._timer);
  this._timer = undefined;
...
```



# <a name="apidoc.module.ssh2.utils"></a>[module ssh2.utils](#apidoc.module.ssh2.utils)

#### <a name="apidoc.element.ssh2.utils.DSAKeySSHToASN1"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>DSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.DSAKeySSHToASN1)
- description and source-code
```javascript
function DSAKeySSHToASN1(key, self, callback) {
  // Convert SSH key parameters to ASN.1 BER values for OpenSSL
  var p = readString(key, key._pos, self, callback);
  if (p === false)
    return false;
  var q = readString(key, key._pos, self, callback);
  if (q === false)
    return false;
  var g = readString(key, key._pos, self, callback);
  if (g === false)
    return false;
  var y = readString(key, key._pos, self, callback);
  if (y === false)
    return false;

  var asnWriter = new Ber.Writer();
  asnWriter.startSequence();
    // algorithm
    asnWriter.startSequence();
      asnWriter.writeOID('1.2.840.10040.4.1'); // id-dsa
      // algorithm parameters
      asnWriter.startSequence();
        asnWriter.writeBuffer(p, Ber.Integer);
        asnWriter.writeBuffer(q, Ber.Integer);
        asnWriter.writeBuffer(g, Ber.Integer);
      asnWriter.endSequence();
    asnWriter.endSequence();

    // subjectPublicKey
    asnWriter.startSequence(Ber.BitString);
      asnWriter.writeByte(0x00);
      asnWriter.writeBuffer(y, Ber.Integer);
    asnWriter.endSequence();
  asnWriter.endSequence();
  return asnWriter.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.DSASigBERToBare"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>DSASigBERToBare (signature)](#apidoc.element.ssh2.utils.DSASigBERToBare)
- description and source-code
```javascript
function DSASigBERToBare(signature) {
  if (signature.length <= 40)
    return signature;
  // This is a quick and dirty way to get from BER encoded r and s that
  // OpenSSL gives us, to just the bare values back to back (40 bytes
  // total) like OpenSSH (and possibly others) are expecting
  var asnReader = new Ber.Reader(signature);
  asnReader.readSequence();
  var r = asnReader.readString(Ber.Integer, true);
  var s = asnReader.readString(Ber.Integer, true);
  var rOffset = 0;
  var sOffset = 0;
  if (r.length < 20) {
    var rNew = new Buffer(20);
    r.copy(rNew, 1);
    r = rNew;
    r[0] = 0;
  }
  if (s.length < 20) {
    var sNew = new Buffer(20);
    s.copy(sNew, 1);
    s = sNew;
    s[0] = 0;
  }
  if (r.length > 20 && r[0] === 0x00)
    rOffset = 1;
  if (s.length > 20 && s[0] === 0x00)
    sOffset = 1;
  var newSig = new Buffer((r.length - rOffset) + (s.length - sOffset));
  r.copy(newSig, 0, rOffset);
  s.copy(newSig, r.length - rOffset, sOffset);
  return newSig;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.DSASigBareToBER"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>DSASigBareToBER (signature)](#apidoc.element.ssh2.utils.DSASigBareToBER)
- description and source-code
```javascript
function DSASigBareToBER(signature) {
  if (signature.length > 40)
    return signature;
  // Change bare signature r and s values to ASN.1 BER values for OpenSSL
  var asnWriter = new Ber.Writer();
  asnWriter.startSequence();
  var r = signature.slice(0, 20);
  var s = signature.slice(20);
  if (r[0] & 0x80) {
    var rNew = new Buffer(21);
    rNew[0] = 0x00;
    r.copy(rNew, 1);
    r = rNew;
  } else if (r[0] === 0x00 && !(r[1] & 0x80)) {
    r = r.slice(1);
  }
  if (s[0] & 0x80) {
    var sNew = new Buffer(21);
    sNew[0] = 0x00;
    s.copy(sNew, 1);
    s = sNew;
  } else if (s[0] === 0x00 && !(s[1] & 0x80)) {
    s = s.slice(1);
  }
  asnWriter.writeBuffer(r, Ber.Integer);
  asnWriter.writeBuffer(s, Ber.Integer);
  asnWriter.endSequence();
  return asnWriter.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.ECDSAKeySSHToASN1"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.ECDSAKeySSHToASN1)
- description and source-code
```javascript
function ECDSAKeySSHToASN1(key, self, callback) {
  // Convert SSH key parameters to ASN.1 BER values for OpenSSL
  var curve = readString(key, key._pos, self, callback);
  if (curve === false)
    return false;
  var Q = readString(key, key._pos, self, callback);
  if (Q === false)
    return false;

  var ecCurveOID;
  switch (curve.toString('ascii')) {
    case 'nistp256':
      // prime256v1/secp256r1
      ecCurveOID = '1.2.840.10045.3.1.7';
      break;
    case 'nistp384':
      // secp384r1
      ecCurveOID = '1.3.132.0.34';
      break;
    case 'nistp521':
      // secp521r1
      ecCurveOID = '1.3.132.0.35';
      break;
    default:
      return false;
  }
  var asnWriter = new Ber.Writer();
  asnWriter.startSequence();
    // algorithm
    asnWriter.startSequence();
      asnWriter.writeOID('1.2.840.10045.2.1'); // id-ecPublicKey
      // algorithm parameters (namedCurve)
      asnWriter.writeOID(ecCurveOID);
    asnWriter.endSequence();

    // subjectPublicKey
    asnWriter.startSequence(Ber.BitString);
      asnWriter.writeByte(0x00);
      // XXX: hack to write a raw buffer without a tag -- yuck
      asnWriter._ensure(Q.length);
      Q.copy(asnWriter._buf, asnWriter._offset, 0, Q.length);
      asnWriter._offset += Q.length;
      // end hack
    asnWriter.endSequence();
  asnWriter.endSequence();
  return asnWriter.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.ECDSASigASN1ToSSH"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSASigASN1ToSSH (signature)](#apidoc.element.ssh2.utils.ECDSASigASN1ToSSH)
- description and source-code
```javascript
function ECDSASigASN1ToSSH(signature) {
  if (signature[0] === 0x00)
    return signature;
  // Convert SSH signature parameters to ASN.1 BER values for OpenSSL
  var asnReader = new Ber.Reader(signature);
  asnReader.readSequence();
  var r = asnReader.readString(Ber.Integer, true);
  var s = asnReader.readString(Ber.Integer, true);
  if (r === null || s === null)
    throw new Error('Invalid signature');
  var newSig = new Buffer(4 + r.length + 4 + s.length);
  newSig.writeUInt32BE(r.length, 0, true);
  r.copy(newSig, 4);
  newSig.writeUInt32BE(s.length, 4 + r.length, true);
  s.copy(newSig, 4 + 4 + r.length);
  return newSig;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.ECDSASigSSHToASN1"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>ECDSASigSSHToASN1 (signature, self, callback)](#apidoc.element.ssh2.utils.ECDSASigSSHToASN1)
- description and source-code
```javascript
function ECDSASigSSHToASN1(signature, self, callback) {
  // Convert SSH signature parameters to ASN.1 BER values for OpenSSL
  var r = readString(signature, 0, self, callback);
  if (r === false)
    return false;
  var s = readString(signature, signature._pos, self, callback);
  if (s === false)
    return false;

  var asnWriter = new Ber.Writer();
  asnWriter.startSequence();
  asnWriter.writeBuffer(r, Ber.Integer);
  asnWriter.writeBuffer(s, Ber.Integer);
  asnWriter.endSequence();
  return asnWriter.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.RSAKeySSHToASN1"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>RSAKeySSHToASN1 (key, self, callback)](#apidoc.element.ssh2.utils.RSAKeySSHToASN1)
- description and source-code
```javascript
function RSAKeySSHToASN1(key, self, callback) {
  // Convert SSH key parameters to ASN.1 BER values for OpenSSL
  var e = readString(key, key._pos, self, callback);
  if (e === false)
    return false;
  var n = readString(key, key._pos, self, callback);
  if (n === false)
    return false;

  var asnWriter = new Ber.Writer();
  asnWriter.startSequence();
    // algorithm
    asnWriter.startSequence();
      asnWriter.writeOID('1.2.840.113549.1.1.1'); // rsaEncryption
      // algorithm parameters (RSA has none)
      asnWriter.writeNull();
    asnWriter.endSequence();

    // subjectPublicKey
    asnWriter.startSequence(Ber.BitString);
      asnWriter.writeByte(0x00);
      asnWriter.startSequence();
        asnWriter.writeBuffer(n, Ber.Integer);
        asnWriter.writeBuffer(e, Ber.Integer);
      asnWriter.endSequence();
    asnWriter.endSequence();
  asnWriter.endSequence();
  return asnWriter.buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.convertPPKPrivate"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>convertPPKPrivate (keyInfo)](#apidoc.element.ssh2.utils.convertPPKPrivate)
- description and source-code
```javascript
function convertPPKPrivate(keyInfo) {
  if (!keyInfo.ppk || !keyInfo.public || !keyInfo.private)
    throw new Error("Key isn't a PPK");
  else if (keyInfo._converted)
    return false;

  var pub = keyInfo.public;
  var priv = keyInfo.private;
  var asnWriter = new Ber.Writer();
  var p;
  var q;

  if (keyInfo.type === 'rsa') {
    var e = readString(pub, 4 + 7);
    var n = readString(pub, pub._pos);
    var d = readString(priv, 0);
    p = readString(priv, priv._pos);
    q = readString(priv, priv._pos);
    var iqmp = readString(priv, priv._pos);
    var p1 = new BigInteger(p, 256);
    var q1 = new BigInteger(q, 256);
    var dmp1 = new BigInteger(d, 256);
    var dmq1 = new BigInteger(d, 256);

    dmp1 = new Buffer(dmp1.mod(p1.subtract(BigInteger.ONE)).toByteArray());
    dmq1 = new Buffer(dmq1.mod(q1.subtract(BigInteger.ONE)).toByteArray());

    asnWriter.startSequence();
      asnWriter.writeInt(0x00, Ber.Integer);
      asnWriter.writeBuffer(n, Ber.Integer);
      asnWriter.writeBuffer(e, Ber.Integer);
      asnWriter.writeBuffer(d, Ber.Integer);
      asnWriter.writeBuffer(p, Ber.Integer);
      asnWriter.writeBuffer(q, Ber.Integer);
      asnWriter.writeBuffer(dmp1, Ber.Integer);
      asnWriter.writeBuffer(dmq1, Ber.Integer);
      asnWriter.writeBuffer(iqmp, Ber.Integer);
    asnWriter.endSequence();
  } else {
    p = readString(pub, 4 + 7);
    q = readString(pub, pub._pos);
    var g = readString(pub, pub._pos);
    var y = readString(pub, pub._pos);
    var x = readString(priv, 0);

    asnWriter.startSequence();
      asnWriter.writeInt(0x00, Ber.Integer);
      asnWriter.writeBuffer(p, Ber.Integer);
      asnWriter.writeBuffer(q, Ber.Integer);
      asnWriter.writeBuffer(g, Ber.Integer);
      asnWriter.writeBuffer(y, Ber.Integer);
      asnWriter.writeBuffer(x, Ber.Integer);
    asnWriter.endSequence();
  }

  var b64key = asnWriter.buffer.toString('base64').replace(RE_KEY_LEN, '$1\n');
  var fullkey = '-----BEGIN '
                + (keyInfo.type === 'rsa' ? 'RSA' : 'DSA')
                + ' PRIVATE KEY-----\n'
                + b64key
                + (b64key[b64key.length - 1] === '\n' ? '' : '\n')
                + '-----END '
                + (keyInfo.type === 'rsa' ? 'RSA' : 'DSA')
                + ' PRIVATE KEY-----';

  keyInfo.private = asnWriter.buffer;
  keyInfo.privateOrig = new Buffer(fullkey);
  keyInfo._converted = true;
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.decryptKey"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>decryptKey (keyInfo, passphrase)](#apidoc.element.ssh2.utils.decryptKey)
- description and source-code
```javascript
function decryptKey(keyInfo, passphrase) {
  if (keyInfo._decrypted || !keyInfo.encryption)
    return;

  var keylen = 0;
  var key;
  var iv;
  var dc;

  keyInfo.encryption = (SSH_TO_OPENSSL[keyInfo.encryption]
                        || keyInfo.encryption);
  switch (keyInfo.encryption) {
    case 'aes-256-cbc':
    case 'aes-256-ctr':
      keylen = 32;
      break;
    case 'des-ede3-cbc':
    case 'des-ede3':
    case 'aes-192-cbc':
    case 'aes-192-ctr':
      keylen = 24;
      break;
    case 'aes-128-cbc':
    case 'aes-128-ctr':
    case 'cast-cbc':
    case 'bf-cbc':
      keylen = 16;
      break;
    default:
      throw new Error('Unsupported cipher for encrypted key: '
                      + keyInfo.encryption);
  }

  if (keyInfo.ppk) {
    iv = PPK_IV;

    key = Buffer.concat([
      crypto.createHash('sha1')
            .update('\x00\x00\x00\x00' + passphrase, 'utf8')
            .digest(),
      crypto.createHash('sha1')
            .update('\x00\x00\x00\x01' + passphrase, 'utf8')
            .digest()
    ]);
    key = key.slice(0, keylen);
  } else {
    iv = new Buffer(keyInfo.extra[0], 'hex');

    key = crypto.createHash('md5')
                .update(passphrase, 'utf8')
                .update(iv.slice(0, 8))
                .digest();

    while (keylen > key.length) {
      key = Buffer.concat([
        key,
        (crypto.createHash('md5')
               .update(key)
               .update(passphrase, 'utf8')
               .update(iv)
               .digest()).slice(0, 8)
      ]);
    }
    if (key.length > keylen)
      key = key.slice(0, keylen);
  }

  dc = crypto.createDecipheriv(keyInfo.encryption, key, iv);
  dc.setAutoPadding(false);
  keyInfo.private = Buffer.concat([ dc.update(keyInfo.private), dc.final() ]);

  keyInfo._decrypted = true;

  if (keyInfo.privateOrig) {
    // Update our original base64-encoded version of the private key
    var orig = keyInfo.privateOrig.toString('utf8');
    var newOrig = /^(.+(?:\r\n|\n))/.exec(orig)[1];
    var b64key = keyInfo.private.toString('base64');

    newOrig += b64key.match(/.{1,70}/g).join('\n');
    newOrig += /((?:\r\n|\n).+)$/.exec(orig)[1];

    keyInfo.privateOrig = newOrig;
  } else if (keyInfo.ppk) {
    var valid = verifyPPKMAC(keyInfo, passphrase, keyInfo.private);
    if (!valid)
      throw new Error('PPK MAC mismatch');
    // Automatically convert private key data to OpenSSL format
    // (including PEM)
    convertPPKPrivate(keyInfo);
  }

  // Fill in full key type
  // TODO: make DRY, we do this also in keyParser
  if (keyInfo.type !== 'ec') {
    keyInfo.fulltype = 'ssh-' + keyInfo.type;
  } else {
    // ECDSA
    var asnReader = new Ber.Reader(keyInfo.private);
    asnReader.readSequence();
    asnReader.readInt();
    asnReader.readString(Ber.OctetString, true);
    asnReader.readByte(); // Skip "complex" context type byte
    var offset = asnReader.readLength(); // Skip context length
    if (offset !== null) {
      asnReader._offset = offset;
      switch (asnReader.readOID()) {
        case '1.2.840.10045.3.1.7':
          // prime256v1/secp256r1
          keyInfo.fulltype = 'ecdsa-sha2-nistp256';
          break;
        case '1.3.132.0.34':
          // secp384r1
          keyInfo.fulltype = 'ecdsa-sha2-nistp384';
          break;
        case '1.3.132.0.35':
          // secp521r1
          keyInfo.fulltype = 'ecdsa-sha2-nistp521';
          break;
      }
    }
    if (keyInfo.fulltype === undefined)
      return new Error('Unsupported EC private key type');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.genPublicKey"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>genPublicKey (keyInfo)](#apidoc.element.ssh2.utils.genPublicKey)
- description and source-code
```javascript
function genPublicKey(keyInfo) {
  var publicKey;
  var i;

  // RSA
  var n;
  var e;

  // DSA
  var p;
  var q;
  var g;
  var y;

  // ECDSA
  var d;
  var Q;
  var ecCurveOID;
  var ecCurveName;

  if (keyInfo.private) {
    // parsing private key in ASN.1 format in order to generate a public key
    var privKey = keyInfo.private;
    var asnReader = new Ber.Reader(privKey);
    var errMsg;

    if (asnReader.readSequence() === null) {
      errMsg = 'Malformed private key (expected sequence)';
      if (keyInfo._decrypted)
        errMsg += '. Bad passphrase?';
      throw new Error(errMsg);
    }

    // version (ignored)
    if (asnReader.readInt() === null) {
      errMsg = 'Malformed private key (expected version)';
      if (keyInfo._decrypted)
        errMsg += '. Bad passphrase?';
      throw new Error(errMsg);
    }

    if (keyInfo.type === 'rsa') {
      // modulus (n) -- integer
      n = asnReader.readString(Ber.Integer, true);
      if (n === null) {
        errMsg = 'Malformed private key (expected RSA n value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      // public exponent (e) -- integer
      e = asnReader.readString(Ber.Integer, true);
      if (e === null) {
        errMsg = 'Malformed private key (expected RSA e value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      publicKey = new Buffer(4 + 7 // ssh-rsa
                             + 4 + n.length
                             + 4 + e.length);

      publicKey.writeUInt32BE(7, 0, true);
      publicKey.write('ssh-rsa', 4, 7, 'ascii');

      i = 4 + 7;
      publicKey.writeUInt32BE(e.length, i, true);
      e.copy(publicKey, i += 4);

      publicKey.writeUInt32BE(n.length, i += e.length, true);
      n.copy(publicKey, i += 4);
    } else if (keyInfo.type === 'dss') { // DSA
      // prime (p) -- integer
      p = asnReader.readString(Ber.Integer, true);
      if (p === null) {
        errMsg = 'Malformed private key (expected DSA p value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      // group order (q) -- integer
      q = asnReader.readString(Ber.Integer, true);
      if (q === null) {
        errMsg = 'Malformed private key (expected DSA q value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      // group generator (g) -- integer
      g = asnReader.readString(Ber.Integer, true);
      if (g === null) {
        errMsg = 'Malformed private key (expected DSA g value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      // public key value (y) -- integer
      y = asnReader.readString(Ber.Integer, true);
      if (y === null) {
        errMsg = 'Malformed private key (expected DSA y value)';
        if (keyInfo._decrypted)
          errMsg += '. Bad passphrase?';
        throw new Error(errMsg);
      }

      publicKey = new Buffer(4 + 7 // ssh-dss
                             + 4 + p.length
                             + 4 + q.length
                             + 4 + g.length
                             + 4 + y.length);

      publicKey.writeUInt32BE(7, 0, true);
      publicKey.write('ssh-dss', 4, 7, 'ascii');

      i = 4 + 7;
      publicKey.writeUInt32BE(p.length, i, true);
      p.copy(publicKey, i += 4);

      publicKey.writeUInt32BE(q.length, i += p.length, true);
      q.copy(publicKey, i += 4);

      publicKey.writeUInt32BE(g.length, i += q.length, true);
      g.copy(publicKey, i += 4);

      publicKey.writeUInt32BE(y.length, i += g.length, true);
      y.copy(publicKey, i += 4);
    } else { // ECDSA
      d = asnReader.readString(Ber.OctetString, true);
      if (d === null)
        throw new Error('Malformed private key (expected ECDSA private key)');
      asnReader.readByte(); // Skip "complex" context type byte
      var offset = asnReader.readLength(); // Sk ...
```
- example usage
```shell
...
var crypto = require('crypto');
var inspect = require('util').inspect;

var buffersEqual = require('buffer-equal-constant-time');
var ssh2 = require('ssh2');
var utils = ssh2.utils;

var pubKey = utils.genPublicKey(utils.parseKey(fs.readFileSync('user.pub')));

new ssh2.Server({
hostKeys: [fs.readFileSync('host.key')]
}, function(client) {
console.log('Client connected!');

client.on('authentication', function(ctx) {
...
```

#### <a name="apidoc.element.ssh2.utils.isStreamCipher"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>isStreamCipher (name)](#apidoc.element.ssh2.utils.isStreamCipher)
- description and source-code
```javascript
function isStreamCipher(name) {
  return RE_STREAM.test(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.iv_inc"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>iv_inc (iv)](#apidoc.element.ssh2.utils.iv_inc)
- description and source-code
```javascript
function iv_inc(iv) {
  var n = 12;
  var c = 0;
  do {
    --n;
    c = iv[n];
    if (c === 255)
      iv[n] = 0;
    else {
      iv[n] = ++c;
      return;
    }
  } while (n > 4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.parseKey"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>parseKey (data)](#apidoc.element.ssh2.utils.parseKey)
- description and source-code
```javascript
parseKey = function (data) {
  if (Buffer.isBuffer(data))
    data = data.toString('utf8');
  else if (typeof data !== 'string')
    return new Error('Key data must be a Buffer or string');

  var ret = {
    fulltype: undefined,
    type: undefined,
    curve: undefined,
    extra: undefined,
    comment: undefined,
    encryption: undefined,
    private: undefined,
    privateOrig: undefined,
    public: undefined,
    publicOrig: undefined
  };
  var m;
  var i;
  var len;

  data = data.trim().split(/\r\n|\n/);

  while (!data[0].length)
    data.shift();
  while (!data.slice(-1)[0].length)
    data.pop();

  var orig = data.join('\n');

  if ((m = RE_HEADER_OPENSSH_PRIV.exec(data[0]))
      && RE_FOOTER_OPENSSH_PRIV.test(data.slice(-1))) {
    // OpenSSH private key
    var keyType = m[1].toLowerCase();
    if (keyType === 'dsa')
      keyType = 'dss';

    if (keyType === 'ec' && semver.lt(process.version, '5.2.0')) {
      return new Error(
        'EC private keys are not supported in this version of node'
      );
    }

    if (!RE_HEADER_OPENSSH.test(data[1])) {
      // unencrypted, no headers
      var privData = new Buffer(data.slice(1, -1).join(''), 'base64');
      if (keyType !== 'ec') {
        ret.fulltype = 'ssh-' + keyType;
      } else {
        // ECDSA
        var asnReader = new Ber.Reader(privData);
        asnReader.readSequence();
        asnReader.readInt();
        asnReader.readString(Ber.OctetString, true);
        asnReader.readByte(); // Skip "complex" context type byte
        var offset = asnReader.readLength(); // Skip context length
        if (offset !== null) {
          asnReader._offset = offset;
          switch (asnReader.readOID()) {
            case '1.2.840.10045.3.1.7':
              // prime256v1/secp256r1
              ret.fulltype = 'ecdsa-sha2-nistp256';
              break;
            case '1.3.132.0.34':
              // secp384r1
              ret.fulltype = 'ecdsa-sha2-nistp384';
              break;
            case '1.3.132.0.35':
              // secp521r1
              ret.fulltype = 'ecdsa-sha2-nistp521';
              break;
          }
        }
        if (ret.fulltype === undefined)
          return new Error('Unsupported EC private key type');
      }
      ret.private = privData;
    } else {
      // possibly encrypted, headers
      for (i = 1, len = data.length; i < len; ++i) {
        m = RE_HEADER_OPENSSH.exec(data[i]);
        if (m) {
          m[1] = m[1].toLowerCase();
          if (m[1] === 'dek-info') {
            m[2] = m[2].split(',');
            ret.encryption = m[2][0].toLowerCase();
            if (m[2].length > 1)
              ret.extra = m[2].slice(1);
          }
        } else if (data[i].length)
          break;
      }
      ret.private = new Buffer(data.slice(i, -1).join(''), 'base64');
    }
    ret.type = keyType;
    ret.privateOrig = new Buffer(orig);
  } else if (m = RE_HEADER_OPENSSH_PUB.exec(data[0])) {
    // OpenSSH public key
    ret.fulltype = m[1];
    ret.type = (m[2] || 'ec').toLowerCase();
    ret.public = new Buffer(m[4], 'base64');
    ret.publicOrig = new Buffer(orig);
    ret.comment = m[5];
    if (m[3]) // ECDSA only
      ret.curve = 'nistp' + m[3];
  } else if (RE_HEADER_RFC4716_PUB.test(data[0])
             && RE_FOOTER_RFC4716_PUB.test(data.slice(-1))) {
    if (data[1].indexOf(': ') === -1) {
      // no headers
      ret.public = new Buffer(data.slice(1, -1).join(''), 'base64');
    } else {
      // headers
      for (i = 1, len = data.length; i < len; ++i) {
        if (data[i].indexOf(': ') === -1) {
          if (data[i].length)
            break; // start of key data
          else
            continue; // empty line
        }
        while (data[i].substr(-1) === '\\') {
          if (i + 1 < len) {
            data[i] = data[i].slice(0, -1) + data[i + 1];
            data.splice(i + 1, 1);
            --len;
          } else
            return new Error('RFC4716 public key missing header continuation line');
        }
        m = RE_HEADER_RFC4716.exec(data[i]);
        if (m) {
          m[1] = m[1].toLo ...
```
- example usage
```shell
...
var crypto = require('crypto');
var inspect = require('util').inspect;

var buffersEqual = require('buffer-equal-constant-time');
var ssh2 = require('ssh2');
var utils = ssh2.utils;

var pubKey = utils.genPublicKey(utils.parseKey(fs.readFileSync('user.pub')));

new ssh2.Server({
hostKeys: [fs.readFileSync('host.key')]
}, function(client) {
console.log('Client connected!');

client.on('authentication', function(ctx) {
...
```

#### <a name="apidoc.element.ssh2.utils.readInt"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>readInt (buffer, start, stream, cb)](#apidoc.element.ssh2.utils.readInt)
- description and source-code
```javascript
function readInt(buffer, start, stream, cb) {
  var bufferLen = buffer.length;
  if (start < 0 || start >= bufferLen || (bufferLen - start) < 4) {
    stream && stream._cleanup(cb);
    return false;
  }

  return buffer.readUInt32BE(start, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.readString"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>readString (buffer, start, encoding, stream, cb, maxLen)](#apidoc.element.ssh2.utils.readString)
- description and source-code
```javascript
function readString(buffer, start, encoding, stream, cb, maxLen) {
  if (encoding && !Buffer.isBuffer(encoding) && typeof encoding !== 'string') {
    if (typeof cb === 'number')
      maxLen = cb;
    cb = stream;
    stream = encoding;
    encoding = undefined;
  }

  start || (start = 0);
  var bufferLen = buffer.length;
  var left = (bufferLen - start);
  var len;
  var end;
  if (start < 0 || start >= bufferLen || left < 4) {
    stream && stream._cleanup(cb);
    return false;
  }

  len = buffer.readUInt32BE(start, true);
  if (len > (maxLen || MAX_STRING_LEN) || left < (4 + len)) {
    stream && stream._cleanup(cb);
    return false;
  }

  start += 4;
  end = start + len;
  buffer._pos = end;

  if (encoding) {
    if (Buffer.isBuffer(encoding)) {
      buffer.copy(encoding, 0, start, end);
      return encoding;
    } else
      return buffer.toString(encoding, start, end);
  } else
    return buffer.slice(start, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ssh2.utils.verifyPPKMAC"></a>[function <span class="apidocSignatureSpan">ssh2.utils.</span>verifyPPKMAC (keyInfo, passphrase, privateKey)](#apidoc.element.ssh2.utils.verifyPPKMAC)
- description and source-code
```javascript
function verifyPPKMAC(keyInfo, passphrase, privateKey) {
  if (keyInfo._macresult !== undefined)
    return keyInfo._macresult;
  else if (!keyInfo.ppk)
    throw new Error("Key isn't a PPK");
  else if (!keyInfo.privateMAC)
    throw new Error('Missing MAC');
  else if (!privateKey)
    throw new Error('Missing raw private key data');
  else if (keyInfo.encryption && typeof passphrase !== 'string')
    throw new Error('Missing passphrase for encrypted PPK');
  else if (keyInfo.encryption && !keyInfo._decrypted)
    throw new Error('PPK must be decrypted before verifying MAC');

  var mac = keyInfo.privateMAC;
  var typelen = keyInfo.fulltype.length;
  // encryption algorithm is converted at this point for use with OpenSSL,
  // so we need to use the original value so that the MAC is calculated
  // correctly
  var enc = (keyInfo.encryption ? 'aes256-cbc' : 'none');
  var enclen = enc.length;
  var commlen = Buffer.byteLength(keyInfo.comment);
  var pub = keyInfo.public;
  var publen = pub.length;
  var privlen = privateKey.length;
  var macdata = new Buffer(4 + typelen
                           + 4 + enclen
                           + 4 + commlen
                           + 4 + publen
                           + 4 + privlen);
  var p = 0;

  macdata.writeUInt32BE(typelen, p, true);
  macdata.write(keyInfo.fulltype, p += 4, typelen, 'ascii');
  macdata.writeUInt32BE(enclen, p += typelen, true);
  macdata.write(enc, p += 4, enclen, 'ascii');
  macdata.writeUInt32BE(commlen, p += enclen, true);
  macdata.write(keyInfo.comment, p += 4, commlen, 'utf8');
  macdata.writeUInt32BE(publen, p += commlen, true);
  pub.copy(macdata, p += 4);
  macdata.writeUInt32BE(privlen, p += publen, true);
  privateKey.copy(macdata, p += 4);

  if (typeof passphrase !== 'string')
    passphrase = '';

  var mackey = crypto.createHash('sha1')
                     .update('putty-private-key-file-mac-key', 'ascii')
                     .update(passphrase, 'utf8')
                     .digest();

  var calcMAC = crypto.createHmac('sha1', mackey)
                      .update(macdata)
                      .digest('hex');

  return (keyInfo._macresult = (calcMAC === mac));
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
