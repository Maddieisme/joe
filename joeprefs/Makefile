TARGET := iphone:clang:latest:14.0
ARCHS = arm64 arm64e
include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = joeprefs

joeprefs_FILES = $(wildcard *.m)
joeprefs_FRAMEWORKS = UIKit
joeprefs_PRIVATE_FRAMEWORKS = Preferences
joeprefs_INSTALL_PATH = /Library/PreferenceBundles
joeprefs_LDFLAGS = -install_name /Library/PreferenceBundles/joe.bundle/joe
joeprefs_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk
