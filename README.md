## Filepicker.io Phonegap samples and library
####Setting up your project
Along with the standard Cordova 2.0 base platform, Filepicker.io also requires the ChildBrowser plugin:

- [Childbrowser for iPhone](https://github.com/purplecabbage/phonegap-plugins/tree/master/iPhone/ChildBrowser)
- [Childbrowser for Android](https://github.com/purplecabbage/phonegap-plugins/tree/master/Android/ChildBrowser)

Follow the instructions there to install ChildBrowser. Once ChildBrowser is properly installed, you should be all ready to start!

Just like on the web, copy the Filepicker.io javascript library into your project, include the script tag below, and you'll be all set!

`<script src="filepicker-0.0.1.js"></script>`

Then, you can use all the same calls as with the [Javascript API](https://developers.filepicker.io/docs/web/)!

Be sure to set your api key via the
`filepicker.setKey("MyAPIKey")` call

####Hello World
Once you are set up, getting a file from filepicker.io is as easy as putting an input type in your html:

`<input type="filepicker"/>`

or calling the library directly:

    filepicker.getFile("image/*", function(url, metadata){
        alert("You picked: "+url);
    });

There's so much more, including [saving files](https://developers.filepicker.io/docs/web/#save) and [image conversion](https://developers.filepicker.io/docs/web/#fpurl-images)!

If you have any questions, don't hesitate to reach out to [support@filepicker.io](mailto:support@filepicker.io)

Note that drag-drop functionality is not supported in PhoneGap as mobile phones don't have the required functionality.

Filepicker.io also supports [Javascript](https://developers.filepicker.io/docs/web/), [iOS](https://developers.filepicker.io/docs/ios/), and [Android](https://developers.filepicker.io/docs/android/), and more libraries are being added every week!
*****
