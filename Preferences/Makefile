include $(THEOS)/makefiles/common.mk

export TARGET = iphone:clang:9.3:8.0

BUNDLE_NAME = SafariPlusPrefs
SafariPlusPrefs_CFLAGS = -fobjc-arc
SafariPlusPrefs_FILES = SPPreferenceLocalizationManager.xm preferenceDirectoryPickerNavigationController.xm preferenceDirectoryPickerTableViewController.xm preferenceFileBrowserNavigationController.xm preferenceFileBrowserTableViewController.xm preferenceFileTableViewCell.xm SafariPlusPrefs.m
SafariPlusPrefs_INSTALL_PATH = /Library/PreferenceBundles
SafariPlusPrefs_FRAMEWORKS = UIKit
SafariPlusPrefs_LIBRARIES = colorpicker
SafariPlusPrefs_PRIVATE_FRAMEWORKS = Preferences

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/SafariPlusPrefs.plist$(ECHO_END)
