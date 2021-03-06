<a name="unreleased"></a>
## [Unreleased]


<a name="0.5.6"></a>
## [0.5.6] - 2020-08-12
### fix
- **tests:** pin lua-nginx-module and lua-resty-core [6266c56](https://github.com/fffonion/lua-resty-acme/commit/6266c5651e54c56442cef2584303781d16f84d3a)


<a name="0.5.5"></a>
## [0.5.5] - 2020-06-29
### fix
- **storage:** remove slash in consul and vault key path [5ddf210](https://github.com/fffonion/lua-resty-acme/commit/5ddf21071ce06a7e003a381440ff75df3faff78e)


<a name="0.5.4"></a>
## [0.5.4] - 2020-06-24
### feat
- **vault:** allow overriding tls options in vault storage [fed57b9](https://github.com/fffonion/lua-resty-acme/commit/fed57b9cc2a1d080dd10af398aeb48b1b55874d7)


<a name="0.5.3"></a>
## [0.5.3] - 2020-05-18
### feat
- **storage:** fully implement the file storage backend ([#6](https://github.com/fffonion/lua-resty-acme/issues/6)) [f1183e4](https://github.com/fffonion/lua-resty-acme/commit/f1183e4c4947dad6edd185631358f1d705a2d98e)


<a name="0.5.2"></a>
## [0.5.2] - 2020-04-27
### fix
- ***:** allow API endpoint to include or exclude /directory part [c7feb94](https://github.com/fffonion/lua-resty-acme/commit/c7feb944db40dc7d8e571cc09594aebffc496bd7)


<a name="0.5.1"></a>
## [0.5.1] - 2020-04-25
### fix
- ***:** fix domain key sanity check and http-01 challenge matching [687de21](https://github.com/fffonion/lua-resty-acme/commit/687de2134335278697220cf67ef0b26c4be34e07)
- **client:** better error handling on directory request [984bfad](https://github.com/fffonion/lua-resty-acme/commit/984bfad031cef1a6ee3554c8c736ace596ed10d3)


<a name="0.5.0"></a>
## [0.5.0] - 2020-02-09
### feat
- **client:** implement tls-alpn-01 challenge handler [25dc135](https://github.com/fffonion/lua-resty-acme/commit/25dc135eaf25c604d21b31664bb36e526a72ad2f)

### fix
- **autossl:** add renewal success notice in error log [b1257de](https://github.com/fffonion/lua-resty-acme/commit/b1257de80bb0e55ff70694bba96bbcf9f9507ae8)
- **autossl:** renew uses unparsed pkey [796b6e3](https://github.com/fffonion/lua-resty-acme/commit/796b6e3005b4301371ca99b2573e56644a456f01)
- **client:** catch pkey new error in order_certificate [393a573](https://github.com/fffonion/lua-resty-acme/commit/393a573b3cb7d3c931f3860c4d99e1e5714edb67)
- **client:** refine error message [5aac0fa](https://github.com/fffonion/lua-resty-acme/commit/5aac0fa92b84ba1b483f6c8d6913e67c7722a7cb)


<a name="0.4.2"></a>
## [0.4.2] - 2019-12-17
### fix
- **autossl:** fix lock on different types of keys [09180a2](https://github.com/fffonion/lua-resty-acme/commit/09180a25ea7864e07ef3d94ebb3b8456f072f967)
- **client:** json decode on application/problem+json [2aabc1f](https://github.com/fffonion/lua-resty-acme/commit/2aabc1f5d535f273b97989f5874d45987fa0ebc9)


<a name="0.4.1"></a>
## [0.4.1] - 2019-12-11
### fix
- **client:** log authz final result [52ac754](https://github.com/fffonion/lua-resty-acme/commit/52ac754d8f888ed2f2ffa7976a5c3d6d18e63a48)


<a name="0.4.0"></a>
## [0.4.0] - 2019-12-11
### feat
- ***:** relying on storage to do cluster level sync [b513009](https://github.com/fffonion/lua-resty-acme/commit/b513009154cd8dbefdfe84f85c81c920d4104f9d)

### fix
- **client:** use POST-as-GET pattern [7198557](https://github.com/fffonion/lua-resty-acme/commit/7198557c616ef9f6d7b89809c4eef300a0e690bd)
- **client:** fix parsing challenges [a4a37b5](https://github.com/fffonion/lua-resty-acme/commit/a4a37b572041dc6a1ea2b24ae14b7dea9e30782f)


<a name="0.3.0"></a>
## [0.3.0] - 2019-11-12
### feat
- **storage:** introduce add/setnx api [895b041](https://github.com/fffonion/lua-resty-acme/commit/895b041750ef4e920c3ed8ec432353f8e7e8eced)
- **storage:** add consul and vault storage backend [028daa5](https://github.com/fffonion/lua-resty-acme/commit/028daa5bc965ab10621aa3f16d7ffabe619fd38a)

### fix
- **autossl:** fix typo [7c41e36](https://github.com/fffonion/lua-resty-acme/commit/7c41e36415d13e364fd58b694c3b4066d60ef1f4)
- **renew:** api name in renew [9ecba64](https://github.com/fffonion/lua-resty-acme/commit/9ecba64ad928f4570f0f205459f042c06403efb8)
- **storage:** fix third party storage module test [ef3e110](https://github.com/fffonion/lua-resty-acme/commit/ef3e1107506bfccc843153766ebcae2eee6f82a2)
- **storage:** typo in redis storage, unified interface for file [2dd6cfa](https://github.com/fffonion/lua-resty-acme/commit/2dd6cfa2c77ab36d0254e1fedb832f2ecabcec99)


<a name="0.1.3"></a>
## [0.1.3] - 2019-10-18
### fix
- ***:** compatibility to use in Kong [6cc5688](https://github.com/fffonion/lua-resty-acme/commit/6cc568813d03a5ab8311ebdccf77131c204094d9)
- **openssl:** follow up with upstream openssl library API [e791cb3](https://github.com/fffonion/lua-resty-acme/commit/e791cb302ce04665eaea722e9c0dc2f551f8c829)


<a name="0.1.2"></a>
## [0.1.2] - 2019-09-25
### feat
- **crypto:** ffi support setting subjectAlt [2d992e8](https://github.com/fffonion/lua-resty-acme/commit/2d992e8973e65617d41c2c49dd9cb259deeaf84f)

### fix
- ***:** reduce test flickiness, fix 1-index [706041b](https://github.com/fffonion/lua-resty-acme/commit/706041bec1dd062d6d0114619688c8f289b73779)
- ***:** support openssl 1.0, cleanup error handling [1bb82ad](https://github.com/fffonion/lua-resty-acme/commit/1bb82ada64cab77468878654d324730bd06381e1)
- **openssl:** remove premature error [f1853ab](https://github.com/fffonion/lua-resty-acme/commit/f1853abbb7a0f19a1bf98de99b70fd5b7779985c)
- **openssl:** fix support for OpenSSL 1.0.2 [42c6e1c](https://github.com/fffonion/lua-resty-acme/commit/42c6e1c3de59a24da1b31b03ca517b858417e741)


<a name="0.1.1"></a>
## [0.1.1] - 2019-09-20
### feat
- **autossl:** whitelist domains [3dfc058](https://github.com/fffonion/lua-resty-acme/commit/3dfc05876d5947c869ab2f80cc9ae4e12cf601a8)


<a name="0.1.0"></a>
## 0.1.0 - 2019-09-20
### feat
- ***:** ffi-based openssl backend [ddbc37a](https://github.com/fffonion/lua-resty-acme/commit/ddbc37a227a5855a5a6caa60606d4534363f3204)
- **autossl:** use lrucache [a6999c7](https://github.com/fffonion/lua-resty-acme/commit/a6999c7e154d21ff0b71358735527408836f36a7)
- **autossl:** support ecc certs [6ed6a78](https://github.com/fffonion/lua-resty-acme/commit/6ed6a78e175ba4e6d6511d1c309d239e43b80ef9)
- **crypto:** ffi pkey.new supports DER and public key as well [a18837b](https://github.com/fffonion/lua-resty-acme/commit/a18837b340f612cc4863903d57e5c3f0225c5919)
- **crypto:** ffi openssl supports generating ec certificates [bc9d989](https://github.com/fffonion/lua-resty-acme/commit/bc9d989b4eb8bfa954f2f1ab08b0449957a27402)

### fix
- ***:** cleanup [2e8f3ed](https://github.com/fffonion/lua-resty-acme/commit/2e8f3ed8ac95076537272311338c1256e2a31e67)


[Unreleased]: https://github.com/fffonion/lua-resty-acme/compare/0.5.6...HEAD
[0.5.6]: https://github.com/fffonion/lua-resty-acme/compare/0.5.5...0.5.6
[0.5.5]: https://github.com/fffonion/lua-resty-acme/compare/0.5.4...0.5.5
[0.5.4]: https://github.com/fffonion/lua-resty-acme/compare/0.5.3...0.5.4
[0.5.3]: https://github.com/fffonion/lua-resty-acme/compare/0.5.2...0.5.3
[0.5.2]: https://github.com/fffonion/lua-resty-acme/compare/0.5.1...0.5.2
[0.5.1]: https://github.com/fffonion/lua-resty-acme/compare/0.5.0...0.5.1
[0.5.0]: https://github.com/fffonion/lua-resty-acme/compare/0.4.2...0.5.0
[0.4.2]: https://github.com/fffonion/lua-resty-acme/compare/0.4.1...0.4.2
[0.4.1]: https://github.com/fffonion/lua-resty-acme/compare/0.4.0...0.4.1
[0.4.0]: https://github.com/fffonion/lua-resty-acme/compare/0.3.0...0.4.0
[0.3.0]: https://github.com/fffonion/lua-resty-acme/compare/0.1.3...0.3.0
[0.1.3]: https://github.com/fffonion/lua-resty-acme/compare/0.1.2...0.1.3
[0.1.2]: https://github.com/fffonion/lua-resty-acme/compare/0.1.1...0.1.2
[0.1.1]: https://github.com/fffonion/lua-resty-acme/compare/0.1.0...0.1.1
