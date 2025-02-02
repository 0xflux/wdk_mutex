# 1.0.0

## Additions

Added an idiomatic implementation for FAST_MUTEX.

## Changes

The `Grt` now creates and fetches instances of both a `FastMutex` and a `KMutex` allowing both
mutex types to be stored and accessed globally.

Updated documentation for KMutex to include examples with `Grt` instead of the less ergonomic option of user managed global statics.

# 0.0.5

Version 0.0.5 introduces the Global Reference Tracker, and the `Grt` module which allows you to easily create, track, and use mutexes for a Windows Kernel Driver across all threads and 
callbacks. This improves developer ergonomics in creating, tracking, dropping etc mutexes throughout your drivers codebase.

# 0.0.4

Introduction of two new functions which allow the caller to get owned copy of the protected data (`T`):

- to_owned()
- to_owned_box()

