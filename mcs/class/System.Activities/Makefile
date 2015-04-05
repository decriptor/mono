thisdir = class/System.Activities
SUBDIRS = 
include ../../build/rules.make

LIBRARY = System.Activities.dll
LIB_REFS = System System.Core System.ServiceModel.Internals
LIB_MCS_FLAGS = /unsafe -d:MONO

TEST_MCS_FLAGS = $(LIB_MCS_FLAGS)

EXTRA_DISTFILES =

VALID_PROFILE := $(filter 4, $(FRAMEWORK_VERSION_MAJOR))
ifndef VALID_PROFILE
LIBRARY_NAME = dummy-System.Activities.dll
NO_INSTALL = yes
NO_SIGN_ASSEMBLY = yes
NO_TEST = yes
endif

include ../../build/library.make
