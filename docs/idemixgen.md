Identity Mixer MSP configuration generator (idemixgen)
======================================================

This document describes the usage for the idemixgen utility, which can
be used to create configuration files for the identity mixer based MSP.
Two commands are available, one for creating a fresh CA key pair, and
one for creating an MSP config using a previously generated CA key.

Directory Structure
-------------------

The idemixgen tool will create directories with the following structure:

    - /ca/
        IssuerSecretKey
        IssuerPublicKey
    - /msp/
        IssuerPublicKey
    - /user/
        SignerConfig

The `ca` directory contains the issuer secret key and should only be
present for a CA. The `msp` directory contains the information required
to set up an MSP verifying idemix signatures. The `user` directory
specifies a default signer.

CA Key Generation
-----------------

CA (issuer) keys suitable for identity mixer can be created using
command `idemixgen ca-keygen`. This will create directories `ca` and
`msp` in the working directory.

Adding a Default Signer
-----------------------

After generating the `ca` and `msp` directories with
`idemixgen ca-keygen`, a default signer specified in the `user`
directory can be added to the config with `idemixgen signerconfig`.

    $ idemixgen signerconfig -h
    usage: idemixgen signerconfig [<flags>]

    Generate a default signer for this Idemix MSP

    Flags:
      -h, --help               Show context-sensitive help (also try --help-long and --help-man).
      -u, --org-unit=ORG-UNIT  The Organizational Unit of the default signer
      -a, --admin              Make the default signer admin

For example, we can create a default signer that is a member of
organizational unit \"OrgUnit1\" and that is an admin with the following
command: :

    idemixgen signerconfig -u OrgUnit1 --admin

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>