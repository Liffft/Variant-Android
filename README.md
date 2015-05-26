# Variant-Android

=================

This is currently just a place holder however here are the premises of the library.

* Allow for continuously deployable code without the need for branching strategies
* Allow for development on non ready code
* Allow using the Variant server to enable and disable features remotely
* Allow for custom managed features to be enabled and disabled.


Variant is currently an internal project lib that will be moved here.  Star to keep updated on the progress

It will allow for development flagging of code to allow unfinished code to be in the final code base
while not impacting the the current features.


Current version released basic how-to

1. add to gradle

`compile 'com.liffft:variant:0.0.1'`

2. In your app you need to initial Variant with the application context

`Variant.initialize(this)`

3. In your manifest file add where you use the tokens given to you by the variant server (in progress)


`<meta-data android:name="com.liffft.variant.APPLICATION_TOKEN" android:value="applicationToken" />`

`<meta-data android:name="com.liffft.variant.CLIENT_TOKEN" android:value="clientToken" />`

4. Make sure to have variant_fuse.json and variant_development.json in the main/assests folder

5. You can now use the variant code in your application.

example

`if (Variant.check(FEATURES.SAMPLEA)) //there SAMPLEA = "application.features.featurea"`

Note that the string is just the json notation to a bool value ie {application.features.featurea=true} for the above




