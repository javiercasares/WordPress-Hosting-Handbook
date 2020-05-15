# **WordPress requirements**

- Web Server

- PHP

- - Required PHP extensions
  - Recommended PHP extensions
  - Alternative PHP extensions
  - Upload PHP extensions
  - System Extensions

- Database

- How do I know what version I have?

Although WordPress can work in almost any environment, even very minimal ones, it must be acknowledged that it does not work completely well in these. That's why here we are going to make some minimum recommendations of the environment in which it would work most effectively.

## **Web Server**

The web server is the system where the files of the web site are hosted and where the users arrive to consult them. There are many web servers, and in principle anyone who supports a PHP connection should be able to work with WordPress.

When it comes to the server, web, WordPress works best with these (sorted alphabetically):

- [Apache HTTPD](https://httpd.apache.org/) 2.4.x

- [LiteSpeed Web Server](https://www.litespeedtech.com/products/litespeed-web-server) 5.3.x / 5.4.x

- [nginx](https://nginx.org/) 1.18.x / 1.17x

- [OpenLiteSpeed](https://openlitespeed.org/) 1.7.x / 1.6.x / 1.5.x / 1.4.x

Remember that if you have a website running in production, it is recommended to use the latest stable version of each of the web servers (mainly for security, rather than functionality), but not alpha, beta or candidate (RC) versions.

## PHP

PHP is a programming language on which WordPress code is based. This language runs on the server and it is important to keep it up to date, both for security and mainly for functionality.

WordPress supports many versions of PHP, some already obsolete, but always all that are supported and maintained.

Officially the WordPress core supports from PHP 7.0 to PHP 7.4. However, not all themes or plugins are supported.

When it comes to PHP, WordPress (including its extensions) works best with the following versions:

- [PHP 7.4](https://www.php.net/ChangeLog-7.php#PHP_7_4).x

- [PHP 7.3](https://www.php.net/ChangeLog-7.php#PHP_7_3).x

- [PHP 7.2](https://www.php.net/ChangeLog-7.php#PHP_7_2).x

WordPress does not work with versions less than 7.0. Versions prior to PHP 7.2 are not recommended because it no longer has support of any kind, and only PHP 7.2 if you have the latest version, since it only has security support.

### Required PHP extensions

- [bcmath](https://www.php.net/manual/en/book.bc.php): For arbitrary precision mathematical operations PHP offers the Binary Calculator, which supports numbers of any size and precision, represented as *strings*.
- [curl](https://www.php.net/manual/en/book.curl.php): PHP supports *libcurl*, a library created by Daniel Stenberg that allows you to connect and communicate with different types of servers and different types of protocols.
- [dom](https://www.php.net/manual/en/book.dom.php): Thanks to the Document Object Model, it is possible to manipulate XML documents using the DOM API.
- [exif](https://www.php.net/manual/en/book.exif.php): With the Exif (Exchangeable image information) extension you can work with image metadata.
- [fileinfo](https://www.php.net/manual/en/book.fileinfo.php): The functions in this module try to find out the type of content and the codification of a file by looking for certain *magic* byte sequences in a specific position of the file.
- [hash](https://www.php.net/manual/en/book.hash.php): It is the message encryption engine and allows to improve the direct or incremental security of messages using a variety of hash algorithms.
- [json](https://www.php.net/manual/en/book.json.php): This extension implements the JavaScript Object Notation (JSON) data exchange format.
- [libsodium](https://doc.libsodium.org/): Sodium is a modern, easy-to-use software library for encryption, decryption, signatures, password hashing, and more.
- [mbstring](https://www.php.net/manual/en/book.mbstring.php): Provides specific functions for multibyte text strings and controls character encoding conversion between possible Unicode-based encoding schemes (UTF-8, UTF-16...).
- [mysqli](https://www.php.net/manual/en/book.mysqli.php): The mysqli extension (*mysql improved*) allows access to the functionality provided by MySQL 4.1 and later.
- [mysqlnd](https://www.php.net/manual/en/book.mysqlnd.php): The MySQL Native Driver is a replacement for the MySQL Client Library (libmysqlclient).
- [openssl](https://www.php.net/manual/en/book.openssl.php): This module uses the functions of OpenSSL for generating and verifying signatures and for sealing (encrypting) and opening (decrypting) data.
- [pcre](https://www.php.net/manual/en/book.pcre.php): The PCRE library is a set of functions that implement regular expression pattern comparisons using the same syntax and semantics as Perl 5, with very few differences.
- [xml](https://www.php.net/manual/en/book.xml.php): This set of tools allows to analyze, but not validate, XML documents.

### Recommended PHP extensions

- [filter](https://www.php.net/manual/en/book.filter.php): This extension filters the data either to validate it or to clean it up.
- [iconv](https://www.php.net/manual/en/book.iconv.php): With this module you can convert a string represented by a local character set into one represented by another character set, which can be the Unicode character set.
- [imagick](https://www.php.net/manual/en/book.imagick.php): ImageMagick is a set of software to create, edit and compose bitmap images. It can read, convert and write images in a variety of formats (over 100) including DPX, EXR, GIF, JPEG, JPEG-2000, PDF, PhotoCD, PNG, Postscript, SVG and TIFF.
- [simplexml](https://www.php.net/manual/en/book.simplexml.php): Provides a very simple and easy to use set of tools to convert XML to an object that can be processed with normal property selectors and array iterators.
- [xmlreader](https://www.php.net/manual/en/book.xmlreader.php): The XMLReader extension is an XML parser. The reader acts as a cursor going forward in the document flow and stopping at every node in the path.
- [zip](https://www.php.net/manual/en/book.zip.php): This extension allows reading or writing ZIP archives and the files inside them in a transparent way.

### Alternative PHP extensions

- [gd](https://www.php.net/manual/en/book.image.php): *Alternative to Imagick*. PHP is not limited to creating only HTML output. It can also be used to create and manipulate image files in a variety of different image formats, including GIF, PNG, JPEG, WBMP and XPM.
- [mcrypt](https://www.php.net/manual/en/book.mcrypt.php): *Alternative to libsodium*. This is an interface to the mcrypt library, which supports a variety of block algorithms such as DES, TRipleDES, Blowfish (default), 3-WAY, SAFER-SK64, SAFER-SK128,TWOFISH, TEA, RC2 and GOST in CBC, OFB, CFB and ECB encryption modes.
- [zlib](https://www.php.net/manual/en/book.zlib.php): *Alternative to zip*. This module allows you to read and write gzipped files (.gz) transparently, through the versions of most file system functions that work with gzipped files (and also with uncompressed files, but not with sockets).

### Upload PHP extensions

These extensions are mainly useful in case you have problems with updates, uploading plugins or themes...

- [ftp](https://www.php.net/manual/en/book.ftp.php): This extension is intended for detailed access to an FTP server providing a wide range of controls for the running script.
- [sockets](https://www.php.net/manual/en/book.sockets.php): The socket extension implements a low-level interface for socket communication functions based on the popular BSD sockets, providing the ability to act as both a server and a client to the socket.
- [ssh2](https://www.php.net/manual/en/book.ssh2.php): Links to the libssh2 library which provides access to resources (shell, remote execution, tunneling, file transfer) on a remote machine using a secure cryptographic transport path.

### System Extensions

For some of the PHP extensions to work properly, you will need to install some extra functionality on the operating system you use. In general, Linux servers already have these functions built in as standard, but it is worth checking.

- [ImageMagick](https://imagemagick.org/): Necessary for the Imagick PHP extension to work.
- [Ghost Script](https://www.ghostscript.com/): Allows ImageMagick to generate images from PDF for the Media zone.
- [XDiff](http://www.xmailserver.org/xdiff-lib.html): Implements a basic but complete system of functionalities to create files and patches the binary and text files.

## Database

For data storage, WordPress uses systems based on MySQL distributions, such as MySQL, MariaDB or Percona. All three systems are compatible with WordPress, so at this moment any of the three can be used for its operation.

The use of these versions is recommended, both for performance and security reasons, although previous versions usually work without problems:

- [MariaDB](https://mariadb.org/) 10.4.x / 10.3.x / 10.2.x
- [MySQL](https://dev.mysql.com/downloads/mysql/) 8.0.x / 5.7.x
- [Percona MySQL Server](https://www.percona.com/software/mysql-database/percona-server) 8.0.x / 5.7.x

## How do I know which version I have?

By choosing a web server, PHP and a database you will get your WordPress base installation working at first.


If you already have WordPress installed and want to know what you have, we recommend using the WordPress Community Plugin called [Health Check & Troubleshooting](https://wordpress.org/plugins/health-check/) (more [help for this plugin](https://make.wordpress.org/support/handbook/appendix/troubleshooting-using-the-health-check/)). If you have WordPress 5.2+, the system already has check tools to have that information in the Site Health section (at Tools in the menu).

