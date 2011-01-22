SRC_FILES = \
			../../../../Source/XnFormats/*.cpp

LIB_NAME = XnFormats
USED_LIBS = XnCore OpenNI
DEFINES = XN_FORMATS_EXPORTS

ifneq ($(wildcard /usr/include/jpeglib.h /usr/local/include/jpeglib.h),)
  USED_LIBS += jpeg
else
  INC_DIRS  += ../../../../Source/External/LibJPEG
  SRC_FILES += ../../../../Source/External/LibJPEG/*.c
endif

include ../EngineLibMakefile
