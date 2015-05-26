# Variant-Android

=================

This is currently just a place holder however here are the premises of the library.

1. Allow for continuously deployable code without the need to branching strategies
2. Allow for development on non ready code
3. Allow using the Variant server to enable and disable features remotely
4. Allow for custom managed features to be enabled and disabled.


Variant is currently an internal project lib that will be moved here.  Star to keep updated on the progress

It will allow for development flagging of code to allow unfinished code to be in the final code base
while not impacting the the current features.


Current version released basic how-to

add to gradle

`compile 'com.liffft:variant:0.0.1'`

In your app you need to initial Variant with the application context

`Variant.initialize(this)`

In your manifest file add where you use the tokens given to you by the variant server (in progress)


`<meta-data android:name="com.liffft.variant.APPLICATION_TOKEN" android:value="applicationToken" />`

`<meta-data android:name="com.liffft.variant.CLIENT_TOKEN" android:value="clientToken" />`

Make sure to have variant_fuse.json and variant_development.json in the main/assests folder


