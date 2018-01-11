Getting Started
===============

Install Prerequisites
---------------------

Before we begin, if you haven\'t already done so, you may wish to check
that you have all the [prereqs]{role="doc"} installed on the platform(s)
on which you\'ll be developing blockchain applications and/or operating
Hyperledger Fabric.

Install Binaries and Docker Images
----------------------------------

While we work on developing real installers for the Hyperledger Fabric
binaries, we provide a script that will [binaries]{role="ref"} to your
system. The script also will download the Docker images to your local
registry.

Hyperledger Fabric Samples
--------------------------

We offer a set of sample applications that you may wish to install these
[samples]{role="doc"} before starting with the tutorials as the
tutorials leverage the sample code.

API Documentation
-----------------

The API documentation for Hyperledger Fabric\'s Golang APIs can be found
on the godoc site for
[Fabric](http://godoc.org/github.com/hyperledger/fabric). If you plan on
doing any development using these APIs, you may want to bookmark those
links now.

Hyperledger Fabric SDKs
-----------------------

Hyperledger Fabric intends to offer a number of SDKs for a wide variety
of programming languages. The first two delivered SDKs are the Node.js
and Java SDKs. We hope to provide Python and Go SDKs soon after the
1.0.0 release.

> -   [Hyperledger Fabric Node SDK
>     documentation](https://fabric-sdk-node.github.io/).
> -   [Hyperledger Fabric Java SDK
>     documentation](https://github.com/hyperledger/fabric-sdk-java).

Hyperledger Fabric CA
---------------------

Hyperledger Fabric provides an optional [certificate authority
service](http://hyperledger-fabric-ca.readthedocs.io/en/latest) that you
may choose to use to generate the certificates and key material to
configure and manage identity in your blockchain network. However, any
CA that can generate ECDSA certificates may be used.

Tutorials
---------

We offer four initial tutorials to get you started with Hyperledger
Fabric. The first is oriented to the Hyperledger Fabric **application
developer**, [write\_first\_app]{role="doc"}. It takes you through the
process of writing your first blockchain application for Hyperledger
Fabric using the Hyperledger Fabric [Node
SDK](https://github.com/hyperledger/fabric-sdk-node).

The second tutorial is oriented towards the Hyperledger Fabric network
operators, [build\_network]{role="doc"}. This one walks you through the
process of establishing a blockchain network using Hyperledger Fabric
and provides a basic sample application to test it out.

Finally, we offer two chaincode tutorials. One oriented to developers,
[chaincode4ade]{role="doc"}, and the other oriented to operators,
[chaincode4noah]{role="doc"}.

**Note: If you have questions not addressed by this documentation, or run into
issues with any of the tutorials, please visit the [questions]{role="doc"}
page for some tips on where to find additional help.**

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>
