## Welcome to Sequence Diagram Themes on GitHub

This repository exists to enable users of 
[Sequence Diagram](https://itunes.apple.com/gb/app/sequence-diagram/id1195426709?mt=12) for macOS to use, share, clone and/or improve themes for the application.

Everything here is free to copy and use courtesy of the [MIT license](https://mabidakun.github.io/sequence-diagram-themes/LICENSE), so go ahead, clone away!

### How do I include a theme in my Sequence Diagram?

Simply add the new `# import-theme` comment keyword, followed by the URL to the scheme file.

**For example:**

```
# import-theme https://mabidakun.github.io/sequence-diagram-themes/yellow-text-field-color-scheme.plist

participant "Sequence Diagram" as MSD
...

```

### How do modify a theme?

The themes are simply text files containing `xml`. More specifically, they are actually XML Plist files, but they are super easy to understand and edit.

**The basic pattern of modification is :-**

1. Clone this repository, so that you'll have your own repo to play with and refer to
2. Copy and rename the existing example theme files
3. Edit your local copy
4. Add and Commit your local copy, to your repo.
5. Push your repo back to `github.com` (or wherever you wish to host your theme files)


**When editing the themes, the most important things to note are:-**

   1. The XML must remain well formed. Each `<element>` has an associated end `</element>`
   2. The field names can not be changed. If you do, they will simply be missing (as far as the application is concerned)
   3. Finally, the `hexColor` fields do not include a preceding `#`, as they would in an HTML document. `000000` is valid, whereas `#000000` is not.
   4. If you get stuck, simply prefix the `# import-theme` keyword with another `#`, to remove your custom theme.


### Having trouble? 


Please check out the in-app documentation, or feel free ping me @ [macSequenceDiagram@mikeOsoft.co.uk](macSequenceDiagram@mikeOsoft.co.uk)


-=[ Mike. O. Abidakun ]=-