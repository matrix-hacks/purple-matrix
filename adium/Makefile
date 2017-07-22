DEFAULT_BUILDCONFIGURATION=Debug

BUILDCONFIGURATION?=$(DEFAULT_BUILDCONFIGURATION)

DEFAULT_ADIUM_PLUGINS_DIR=$(HOME)/Library/Application\ Support/Adium\ 2.0/PlugIns
ADIUM_PLUGINS_DIR?=$(DEFAULT_ADIUM_PLUGINS_DIR)

build:
	xcodebuild -project AdiumMatrix.xcodeproj -configuration $(BUILDCONFIGURATION) build

clean:
	rm -rf ./build

install:
	cp -r ./build/$(BUILDCONFIGURATION)/AdiumMatrix.AdiumLibpurplePlugin $(ADIUM_PLUGINS_DIR)

.PHONY: build clean install
