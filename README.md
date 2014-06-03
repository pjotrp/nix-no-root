nix-no-root
===========

Empowered Nix/Guix without root access. The Nix and Guix package
managers are incredible useful for software deployment, also on
systems where you have no root access. 

If the system has gcc, Perl and a few other build tools it may be
possible to bootstrap  on the target system using
./scripts/nix-bootstrap-home.sh.  Alternatively, provided the $HOME
path is the same, you can actually build on any host with a similar
architecture and running kernel and move the binaries across. Nix is
self-contained and depends on very little. That is important to know!

The basic information came from the [Nix
wiki](https://nixos.org/wiki/How_to_install_nix_in_home_%28on_another_distribution%29).

So far, this is the most successful bootstrap route I tried for Nix,
and I have tried quite a few ways over time. For Guix the upside is
that if Nix works you can simply install Guix from a Nix package.
Very easy. 

So far, I have managed to install Nix with these scripts on a large
CentOS6 compute cluster.  When more people have success stories,
please add that information here.

## CentOS6

  Linux version 2.6.32-431.17.1.el6.x86_64 (mockbuild@c6b8.bsys.dev.centos.org) (gcc version 4.4.7 20120313 (Red Hat 4.4.7-4) (GCC) ) #1 SMP Wed May 7 23:32:49 UTC 2014

