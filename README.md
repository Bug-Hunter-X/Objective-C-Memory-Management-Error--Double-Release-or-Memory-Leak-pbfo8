# Objective-C Memory Management Bug

This repository demonstrates a common memory management bug in Objective-C and its solution. The bug involves improper use of `retain`, `release`, and `autorelease` within a custom class, leading to potential memory leaks or crashes due to double-releasing objects.

## Bug Description

The `bug.m` file contains a `MyObject` class with a property `anotherObject`.  The bug occurs because the `anotherObject` is not properly managed when it's assigned multiple times or released inappropriately.  This can result in either memory leaks (if not released) or crashes (if double-released). 

## Solution

The `bugSolution.m` file shows how to fix this bug using proper memory management techniques, avoiding manual retain/release in favor of ARC (Automatic Reference Counting), where possible or employing strong and weak references. 