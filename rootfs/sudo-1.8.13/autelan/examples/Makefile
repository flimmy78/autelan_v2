#
# Copyright (c) 2014 Todd C. Miller <Todd.Miller@courtesan.com>
#
# Permission to use, copy, modify, and distribute this software for any
# purpose with or without fee is hereby granted, provided that the above
# copyright notice and this permission notice appear in all copies.
#
# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
# WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
# MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
# ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
# WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
# ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
# OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
# ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
#
# examples/Makefile.  Generated from Makefile.in by configure.
#

#### Start of system configuration section. ####

srcdir = .
docdir = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../fakerelease/usr/share/doc
exampledir = $(docdir)/examples
top_builddir = ..
top_srcdir = ..

# Our install program supports extra flags...
INSTALL = $(SHELL) $(top_srcdir)/install-sh -c
INSTALL_OWNER = -o $(install_uid) -g $(install_gid)

# Where to install things...
prefix = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../release/usr
exec_prefix = $(prefix)
bindir = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../release/usr/bin
sbindir = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../release/usr/sbin
sysconfdir = /etc
libexecdir = /usr/lib
datarootdir = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../fakerelease/usr/share
localstatedir = /home/hisisdk/histb_v2/autelan/rootfs/sudo-1.8.13/../../release/var

# User and group ids the installed files should be "owned" by
install_uid = 0
install_gid = 0

#### End of system configuration section. ####

SHELL = /bin/sh

EXAMPLES = $(srcdir)/pam.conf $(srcdir)/sudo.conf $(srcdir)/sudoers \
	   $(srcdir)/syslog.conf
 
VERSION = 1.8.13
PACKAGE_TARNAME = sudo

all: $(EXAMPLES)

Makefile: $(srcdir)/Makefile.in
	(cd $(top_builddir) && ./config.status --file examples/Makefile)

pre-install:

install: install-doc

install-dirs:
	$(SHELL) $(top_srcdir)/mkinstalldirs $(DESTDIR)$(exampledir)

install-binaries:

install-includes:

install-doc: install-dirs
	for f in $(EXAMPLES); do $(INSTALL) $(INSTALL_OWNER) -m 0644 $$f $(DESTDIR)$(exampledir); done

install-plugin:

uninstall:
	-rm -rf	$(DESTDIR)$(exampledir)

cppcheck:

check:

clean:

mostlyclean: clean

distclean: clean
	-rm -rf Makefile

clobber: distclean

realclean: distclean

cleandir: distclean
