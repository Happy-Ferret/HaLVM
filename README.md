The Haskell Lightweight Virtual Machine (HALVM) Source Archive
==============================================================

> The HaLVM is (C) 2008 Galois, Inc., and distributed under a standard,
> three-clause BSD license. Please see the file LICENSE, distributed with
> this software, for specific terms and conditions.

1. What is the HaLVM?
---------------------

The Haskell Lightweight Virtual Machine, or HaLVM, is a port of the Glasgow
Haskell Compiler toolsuite to enable developers to write high-level, lightweight
virtual machines that can run directly on the Xen hypervisor.

While Galois initially designed the HaLVM to allow for quick and easy
prototyping of operating systems components, the HaLVM has grown over time to
allow for a much wider variety of use cases. When connected with the appropriate
libraries, the HaLVM can, for example, operate as a network appliance.

Writing for the Haskell Lightweight Virtual Machine is just like writing
normal Haskell, and many pure Haskell libraries port to the HaLVM with little
or no difficulty. In fact, we include the standard
[Haskell Cabal toolset](http://www.haskell.org/cabal/) in order to more easily
facilitate the integration of outside Haskell libraries. However, instead of
running on top of a typical operating system, HaLVM programs run at a very low
level, directly on the Xen hypervisor. This allows for very lightweight, single
purpose Xen domains with minimal resource requirements.

2. Getting and Building the HaLVM
---------------------------------

For those who want to set up a development environment and maybe contribute to HaLVM, please see [HACKING.md](HACKING.md).

In addition, you might want to check out Darrin Eden's build system,
available on GitHub:

    https://github.com/dje/halvm-test

It may provide some information that you'd find useful, or may automate portions of this process for you.


3. Where To Look Next
---------------------

The HaLVM comes with a number of examples / test cases, located in the folder
`examples`. We suggest taking a look at these to see a wide variety of HaLVM
programs you might use as a starting point.

Further information about using the HaLVM is available on the HaLVM wiki.
Developers interested in improving the HaLVM should also take a look at the
current list of HaLVM bugs, and submit any new feature requests to the
HaLVM bug system.

4. How To Contact Us
--------------------

The HaLVM is a proud member of the [unikernel.org](http://unikernel.org)
community. If you have any questions, suggestions, or comments about the HaLVM,
we suggest participation in [devel.unikernel.org](https://devel.unikernel.org),
a multi-unikernel developer's message board.

If you have bugs you would like to file or patches you'd like to send, we'd
strongly prefer you utilize GitHub's interfaces for both these functions. Please
see GitHub for more information.

That's all, and enjoy using the HaLVM!
