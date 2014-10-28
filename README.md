Breakwater
==========

Deobfuscates Jetty passwords.

Usage
-----

If you've ever come across `.htaccess`, `.properties` or `.xml` files 
with the following syntax:

    username: OBF:1vny1zlo1x8e1vnw1vn61x8g1zlu1vn4,authorized

you may know that it means that the password is [obfuscated] [1].

This tool deobfuscates passwords (or any other strings, really) obfuscated
with the standard Jetty password protection scheme:

    ./breakwater 1vny1zlo1x8e1vnw1vn61x8g1zlu1vn4
    storepwd

That's all.

Licence
-------

MIT.

[1]: http://www.eclipse.org/jetty/documentation/current/configuring-security-secure-passwords.html