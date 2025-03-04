<h1 align=center>JuicyFx ZEIT Now PHP</h1>

<p align=center>
Enjoyable & powerful 🐘 PHP builder for ZEIT Now.
</p>

<p align=center>
🕹 <a href="https://f3l1x.io">f3l1x.io</a> | 💻 <a href="https://github.com/f3l1x">f3l1x</a> | 🐦 <a href="https://twitter.com/xf3l1x">@xf3l1x</a>
</p>

## 🤗 Features

- **Architecture**: PHP development server (🚀 fast enought)
- **PHP version**: 7.3.7
- **Extensions**: apcu, bcmath, bz2, calendar, Core, ctype, curl, date, dom, ds, exif, fileinfo, filter, ftp, gettext, hash, iconv, json, libxml, mbstring, mysqli, mysqlnd, openssl, pcntl, pcre, PDO, pdo_mysql, pdo_pgsql, pdo_sqlite, phalcon, Phar, readline, Reflection, session, SimpleXML, soap, sockets, sodium, SPL, sqlite3, ssh2, standard, swoole, tokenizer, xml, xmlreader, xmlrpc, xmlwriter, xsl, Zend OPcache, zlib
- **Speed**: cold ~250ms / warm ~5ms
- **Memory**: ~90mb

> List of all installable extensions is on this page https://blog.remirepo.net/pages/PECL-extensions-RPM-status.

> Need to know how things are changing? Here is [changelog](./CHANGELOG.md).

## ⚙️ Usage

```json
{
  "version": 2,
  "builds": [
    { "src": "index.php", "use": "now-php@canary" }
  ]
}
```

> 🚧Everything is HOT right now, so you should rather test the `now-php@canary` version.

Composer is detected by presence of file `composer.json`. You can force it defining `config.composer` for the build.

```json
{
  "version": 2,
  "builds": [
    { "src": "index.php", "use": "now-php@canary", "config": { "composer": true } }
  ]
}
```

## 👨‍💻`now dev`

For running `now dev` properly, you need to have PHP installed on your computer, [learn more](errors/now-dev-no-local-php.md).

## 👀 Examples

- phpinfo - https://now-php-version.juicyfx1.now.sh
- extensions - https://now-php-ext.juicyfx1.now.sh

![](docs/phpinfo.png)

Browse [more examples](examples). 👀

## 🚧 Roadmap

- next-gen PHP builder ✅
- Composer
  - config.composer: true ✅
  - composer.json detection ✅
- zero config ✅
- `now dev` ✅
- rewrite to typescript ✅

**Help wanted**

- create many examples (majority frameworks and other use-cases)
- cover by tests

## 👨🏻‍💻CHANGELOG

[Browser the changes...](./CHANGELOG.md)

## 📝 License

Copyright © 2019 [f3l1x](https://github.com/f3l1x).
This project is [MIT](LICENSE) licensed.
