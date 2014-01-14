Parse.framework
===============

http://www.parse.com - Parse iOS Framework

Note
----

I couldn't find a repository for this framework (Did I just miss it?), and it's pretty large to include in GitHub repos; so, hopefully, this will allow you to use Parse.framework as a submodule.

iOS / OS X Changelog
--------------------



**v1.2.18 — January 6, 2014**

Removes dependence on SBJSON library.

Adds ```relationForKey``` as a replacement for ```relationforKey```.

**v1.2.17 — December 13, 2013**

Improves support for Facebook iOS SDK v3.10

**v1.2.16 — November 14, 2013**

Add ```isDirty``` and ```isDirtyForKey:``` to ```PFObject```.
Add become APIs to ```PFUser```.

**v1.2.15 — September 23, 2013**

Adds support for 64-bit iOS applications.

**v1.2.14 — September 19, 2013**

Fix some lock contention on the current user that was causing deadlocks when logged in and accessing Parse from a large number of threads.

**v1.2.13 — September 5, 2013**

Adds Custom Analytics tracking with ```[PFAnalytics trackEvent:dimensions:]```.

**v1.2.12 — August 21, 2013**

Improved compatibility between ```PFQueryTableViewController``` and yet-to-be-released iOS versions.
Improves integration with the Facebook SDK.

**v1.2.11 — July 16, 2013**

Support for ```+[PFObject deleteAll:]```

Upgrades to subclasses of ```PFObject```:

Subclasses now support ```@property (readonly) PFRelation *```.
Object properties can now be deleted by assigning nil to them.
Property syntax will correctly convert a literal null (```NSNull``` in Objective-C) field to a nil property value.
(Bugfix) Subclasses of subclasses will not get a default dynamic implementation when the superclass had an explicit definition. This fixes issues seen by some customers with ```PFInstallation``` subclasses.

**v1.2.10 — June 14, 2013**

Fix a problem with crashing when a ```saveEventually``` is rejected on the server.

**v1.2.9 — May 15, 2013**

Remove implementation details from some headers and deprecate sendToIOS/Android in ```PFPush```. Users who wish to target a specific device type should use a ```PFQuery```.

Ownership
---------

This software is owned by Parse, Inc. or Facebook, Inc., and subject to their [acceptable use policy].

[acceptable use policy]: https://www.parse.com/about/aup
