all: ../../bin/nc

../../bin/nc: libs/armeabi/nc
	cp $< $@

libs/armeabi/nc: netcat.c Android.mk
	$(NDK_ROOT)/ndk-build NDK_APPLICATION_MK=`pwd`/Application.mk NDK_APP_OUT=. TARGET_PLATFORM=android-21

clean:
	rm -Rf libs
	rm -Rf local
