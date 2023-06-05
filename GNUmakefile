default:
	type -P rake && rake || echo "command: rake not found...\nTrying: 'gem install rake'" && gem install rake
	$(MAKE) file_check
file_check:
	type -P file && file build-arm/libStaticLibDemo.a
	type -P file && file build-arm64/libStaticLibDemo.a
	type -P file && file build-i386/libStaticLibDemo.a
	type -P file && file build-x86_64/libStaticLibDemo.a