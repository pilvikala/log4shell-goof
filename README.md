# pilvikala-log4shell-goof

This is a demo repository containing exaples of `jar` packages that can be detected as vulnerable to the Log4Shell vulnerability using the `snyk log4shell` command.
See https://docs.snyk.io/features/snyk-cli/test-for-vulnerabilities/how-to-use-the-log4shell-command for more information on how to use `snyk log4shell`.

Example output:

```
$ snyk log4shell
Please note this command is for already built artifacts. To test source code please use `snyk test`.

Results:
A version of Log4J that is vulnerable to Log4Shell was detected:
	./fat-2.15.jar/core/org/apache/logging/log4j/core
	./log4j-core-2.0-rc1.jar
	./nested.jar/log4j-core-2.14.1.jar
	./opencast-search-9.9.jar/log4j-core-2.11.1.jar
	./opencast-search-9.9.jar/org/apache/logging/log4j/core

We highly recommend fixing this vulnerability. If it cannot be fixed by upgrading, see mitigation information here:
      	- https://security.snyk.io/vuln/SNYK-JAVA-ORGAPACHELOGGINGLOG4J-2314720
      	- https://snyk.io/blog/log4shell-remediation-cheat-sheet/
```
