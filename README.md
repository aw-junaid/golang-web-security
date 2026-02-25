# Golang Web Security
<img align="" src="https://github.com/aw-junaid/aw-junaid/blob/main/Assets/asset5.webp" width="1000" height="150" alt="awjunaid">

![GitHub commit activity](https://img.shields.io/github/commit-activity/t/aw-junaid/golang-web-security)
![GitHub contributors](https://img.shields.io/github/contributors/aw-junaid/golang-web-security)
![GitHub repo size](https://img.shields.io/github/repo-size/aw-junaid/golang-web-security)

Secure Golang web app with best practices: authentication, authorization, input validation, CSRF protection, and secure headers. Example code for secure development.

## Contact With Me:

<div align="left">
  <a href="https://www.youtube.com/@awjunaid/featured" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="youtube logo"  />
  </a>
  <a href="https://www.instagram.com/awjunaid_" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="instagram logo"  />
  </a>
  <a href="https://www.twitch.tv/awjunaid" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitch&logo=twitch&label=&color=9146FF&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="twitch logo"  />
  </a>
  <a href="mailto:abdulwahabjunaid07@gmail.com" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="gmail logo"  />
  </a>
  <a href="https://www.linkedin.com/in/aw-junaid" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="linkedin logo"  />
  </a>
  <a href="https://twitter.com/awjunaid_" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitter&logo=twitter&label=&color=1DA1F2&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="twitter logo"  />
  </a>
  <a href="https://discord.gg/Neddn8gPqY" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="discord logo"  />
  </a>
</div>

## 💰 You can help me by Donating
  [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/awjunaid)

## Table of Contents
- [Tools](#tools)
  - [Web Framework Hardening](#web-framework-hardening)
  - [Security Libraries](#security-libraries)
  - [Static Code Analysis](#static-code-analysis)
  - [Vulnerabilities and Security Advisories](#vulnerabilities-and-security-advisories)
  - [Private Key Infrastructure](#private-key-infrastructure)
- [Educational](#educational)
  - [Hacking Playgrounds](#hacking-playgrounds)
  - [Articles, Guides & Talks](#articles-guides--talks)
  - [Reporting Bugs](#reporting-bugs)
- [License](#license)

# Tools

## Web Framework Hardening

*Middleware and utilities to secure your Go web applications at the framework level.*

- [nosurf](https://github.com/justinas/nosurf) - CSRF protection middleware for Go.
- [gorilla/csrf](https://github.com/gorilla/csrf) - Provides Cross-Site Request Forgery (CSRF) prevention middleware for Go web applications & services.
- [gorilla/securecookie](https://github.com/gorilla/securecookie) - Encodes and decodes authenticated and optionally encrypted cookie values for Go web applications.
- [secure](https://github.com/unrolled/secure) - Secure is an HTTP middleware for Go that facilitates most of your security needs for web applications (e.g., HSTS, CSP, etc.).
- [unindexed](https://github.com/jordan-wright/unindexed) - A drop-in replacement for `http.Dir` which disables directory indexing.
- [beego-security-headers](https://github.com/gosecguy/beego-security-headers) - Beego framework filter for easy security headers management.
- [echox/sessions](https://github.com/labstack/echo-contrib/tree/master/sessions) - Secure cookie-based session management for the Echo framework.
- [gin-contrib/secure](https://github.com/gin-contrib/secure) - A Gin middleware for quick implementation of security headers.

## Security Libraries

*General-purpose libraries for implementing specific security controls.*

- [paseto](https://github.com/o1egl/paseto) - Platform-Agnostic Security Tokens implementation in GO (Golang).
- [hsts](https://github.com/StalkR/hsts) - Go HTTP Strict Transport Security library.
- [jwt-go](https://github.com/dgrijalva/jwt-go) - Golang implementation of JSON Web Tokens (JWT). (Note: This library is now archived; it's recommended to look at [golang-jwt/jwt](https://github.com/golang-jwt/jwt) instead).
- [golang-jwt/jwt](https://github.com/golang-jwt/jwt) - A community-maintained fork of the popular `jwt-go` library.
- [httprobe](https://github.com/tomnomnom/httprobe) - Take a list of domains and probe for working HTTP and HTTPS servers (useful for recon).
- [bcrypt](https://pkg.go.dev/golang.org/x/crypto/bcrypt) - The official Go implementation of bcrypt for password hashing.
- [scrypt](https://pkg.go.dev/golang.org/x/crypto/scrypt) - The official Go implementation of the scrypt key derivation function.
- [argon2](https://pkg.go.dev/golang.org/x/crypto/argon2) - The official Go implementation of the Argon2 key derivation function (password hashing).
- [acmetool](https://github.com/hlandau/acme) - An easy-to-use command-line tool for automatically getting TLS certificates from Let's Encrypt.

## Static Code Analysis

*Tools to analyze your source code for potential security flaws.*

- [safesql](https://github.com/stripe/safesql) - Static analysis tool for Golang that protects against SQL injections. It does not seem to be actively maintained at the moment.
- [gosec](https://github.com/securego/gosec) - Inspects source code for security problems by scanning the Go AST and matching it with a set of rules. Comes bundled in a Docker container [securego/gosec](https://hub.docker.com/r/securego/gosec).
- [gometalinter](https://github.com/alecthomas/gometalinter) - Concurrently runs most of the existing go linters and normalizes their output. (Consider using [golangci-lint](https://github.com/golangci/golangci-lint) as a more modern and faster alternative).
- [golangci-lint](https://github.com/golangci-lint/golangci-lint) - A fast Go linters runner. It runs many linters in parallel, including `gosec`, and can be integrated into your CI/CD pipeline.
- [CodeQL](https://securitylab.github.com/tools/codeql) - A tool that lets you query your code like data, in order to find vulnerabilities and bugs. See also [LGTM.com](https://lgtm.com) for pull request integration and running queries in the cloud. (Note: LGTM.com has been sunset, but CodeQL remains available).
- [ChainJacking](https://github.com/Checkmarx/chainjacking) - Find which of your Go lang direct GitHub dependencies is susceptible to ChainJacking attack.
- [Semgrep](https://semgrep.dev/) - A fast, open-source static analysis tool that supports Go and can be used to find security issues by writing custom rules.

## Vulnerabilities and Security Advisories

*Sources for staying informed about known vulnerabilities in Go and its ecosystem.*

- [golang-announce](https://groups.google.com/forum/#!forum/golang-announce) - The golang release mailing list. Language-specific security issues are announced here.
- [Go Vulnerability Database](https://vuln.go.dev/) - The official Go vulnerability database, maintained by the Go team.
- [GoCenter Security](https://jfrog.com/blog/gocenter-reveals-go-module-vulnerabilities-with-xray/) and [JFrog VSCode Extension for Go](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-vscode-extension) - Free vulnerability data around Go Modules.
- [snyk Vulnerability DB](https://snyk.io/vuln?type=golang) - Commercial but free listing of known vulnerabilities in libraries.
- [Common Vulnerabilities and Exposures](https://www.cvedetails.com/vulnerability-list/vendor_id-14185/Golang.html) - Vulnerabilities that were assigned a CVE. Covers the language and packages.
- [National Vulnerability Database](https://nvd.nist.gov/vuln/search/results?form_type=Basic&results_type=overview&query=golang&search_type=all) - Golang known vulnerabilities in the National Vulnerability Database.
- [OSV.dev](https://osv.dev/list?q=golang) - A distributed vulnerability database for open source, with good support for Go.

## Private Key Infrastructure

*Tools for managing certificates and PKI.*

- [CloudFlare SSL](https://github.com/cloudflare/cfssl) - CFSSL is CloudFlare's PKI/TLS swiss army knife. It is both a command line tool and an HTTP API server for signing, verifying, and bundling TLS certificates.
- [step-ca](https://github.com/smallstep/certificates) - A private certificate authority (CA) and ACME server for secure automated certificate management.

# Educational

## Hacking Playgrounds

*Intentionally vulnerable applications to practice security testing and exploitation in Go.*

- [govwa](https://github.com/0c34/govwa) - A vulnerable golang application including the most common vulnerabilities found in web applications today.
- [Lambhack](https://github.com/wickett/lambhack) - A very vulnerable serverless application in AWS Lambda.
- [go-dvwa](https://github.com/eze-kiel/go-dvwa) - A Go version of the popular Damn Vulnerable Web Application (DVWA).
- [gin-vulnerable](https://github.com/bloom42/gin-vulnerable) - An intentionally vulnerable API built with the Gin framework for educational purposes.

## Articles, Guides & Talks

*Presentations, written guides, and example projects for secure Go development.*

- [gosea](https://github.com/komand/gosea) - Go Secure Example Application (GOSEA).
- [Go - Secure Coding Practices](https://www.owasp.org/images/2/2b/Owasp-171123063052.pdf) by OWASP - [PDF] Talk given by Sulhaedir at the OWASP Jakarta meetup.
- [OWASP Go - Secure Coding Practices](https://github.com/OWASP/Go-SCP) by Checkmarx - Go programming language secure coding practices guide.
- [Memory Security in golang](https://cryptolosophy.org/memory-security-go/) - Handling data securely in memory.
- [A Go Programmer's Guide to Secure Connections](https://www.youtube.com/watch?v=kxKLYDLzuHA) - [Video] GopherCon 2018, Liz Rice.
- [golang-tls](https://github.com/denji/golang-tls) - Simple Golang HTTPS/TLS Examples.
- [Hacking with Go](https://github.com/parsiya/Hacking-with-Go) - Hacking with Go for security professionals.
- [ReDoS in Go](https://www.checkmarx.com/2018/05/07/redos-go/) by Checkmarx - Diving Deep into Regular Expression Denial of Service (ReDoS) in Go.
- [Attacking Go](https://blog.trailofbits.com/2019/11/07/attacking-go-vr-ttps/): A detailed description on Security assessment techniques for Go projects.
- [The IoC of Go Generics](https://www.arp242.net/go-generics.html) - A discussion on how generics impact code clarity and potential security implications.
- [Practical Go: Building a Secure Web Application](https://www.youtube.com/watch?v=3F5J0oU7K6Y) - [Video] A talk on practical steps for building secure web apps in Go.

## Reporting Bugs

- [Go Security Policy](https://golang.org/security) - How to responsibly report security issues to the Go team.

# License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
