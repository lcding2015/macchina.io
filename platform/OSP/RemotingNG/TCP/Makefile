#
# Makefile
#
# $Id$
#
# Makefile for OSP RemotingNG TCP bundle
#

BUNDLE_TOOL = $(POCO_BASE)/OSP/BundleCreator/$(POCO_HOST_BINDIR)/bundle

include $(POCO_BASE)/build/rules/global

objects = BundleActivator

target         = com.appinf.osp.remotingng.tcp
target_version = 1
target_libs    = PocoRemotingNGTCP PocoRemotingNG PocoOSP PocoNet PocoUtil PocoXML PocoJSON PocoFoundation

postbuild      = $(SET_LD_LIBRARY_PATH) $(BUNDLE_TOOL) -n$(OSNAME) -a$(OSARCH) -o../../bundles TCP.bndlspec

include $(POCO_BASE)/build/rules/dylib
