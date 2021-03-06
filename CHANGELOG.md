# Aparapi Changelog

## 1.4.1

## 1.4.0

* Updated nexus stagin plugin: 1.6.7 -> 1.6.8
* Added Fused Multiply Add support.
* Fixed a bug whereby the library failed to load if OpenCL implementation isnt present, system now loads and falls back to native Java.
* Fixed several mistakes and typos in the various examples.

## 1.3.4

* Updated to aparapi-jni 1.1.2 thus fixing `UnsatisfiedLinkError` which occured only on Windows.

## 1.3.3

* Added several missing math functions that are part of the OpenCL standard: acospi, asinpi, atanpi, atan2pi, cbrt,
  cosh, cospi, exp2, exp10, expm1, log2, log10, log1p, mad, nextafter, sinh, sinpi, tanh, tanpi.
* Fixed "`CXXABI_1.3.8' not found " error encountered on some older systems.
* Fixed a bug where calling createProgram resulted in an exception.
* Changed aparapi JNI load notification into a proper logger message instead of direct to system.out.

## 1.3.2

* Added Windows 64bit support.
* Improved exception message when a native library can't be loaded.

## 1.3.1

* Added full support for OSX.

## 1.3.0

* No longer needs Aparapi JNI library to be installed manually, this is loaded dynmically now.

## 1.2.0

* Kernels of the same class are now eligible to be run on different devices.
* Added method to set execution mode without any fallback.
* Added opencl device method for name.
* Fixed a memory leak.
* Added method for uncached platform retrieval.

## 1.1.2

* Fixed a bug where OpenCL kernels were getting compiled twice.

## 1.1.1

* Fixed a bug where forward references existed when they shouldnt.
* Fixed some bugs where improper directory structure were referenced produced exceptions.

## 1.1.0

* Changed group id and package to com.aparapi
