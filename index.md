# IronToolbar for AHK

<img src="images/preview.gif">

<details>
<summary>Preview #2</summary>
<img src="images/preview_2.gif">
</details>

<a href="docs/docs.md">Documentation</a>

Why Iron?  Two reasons:
1) This class script has turned out pretty solid and reliable.
2) It was a struggle getting there, due to the Toolbar API's "iron will" to defy my attempts to make this not only accessible for AHK v2, but hopefully more accessible and usable if converted to AHK v1.

The latter is my attempt at a light-hearted joke, reflecting on my journey to getting this class script ready for a release.

I designed this class around `tb.easyMode := true`.  EasyMode is on by default and allows maximimum flexibility with minimal code.  If you want, after creating a toolbar object, set `tb.easyMode := false` to have more granular control over adding styles, but you can also exercise more control by simply using `tb.SendMsg()`.  EasyMode takes care of MANY frustrating aspects of managing a toolbar.

For a minimalist example of usage, please see the included example.

Please note that according to the Microsoft docs, the "image index" is always zero-based.  In this script, in true AHK style, the icon index is always 1-based (starting with 1, not zero).  If you decide to send your own messages to the toolbar, when an image index is required, it needs to be zero-based.