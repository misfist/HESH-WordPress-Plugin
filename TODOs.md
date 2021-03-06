# TODOs
- release!

## Testing
- general bugs
	- none currently
- browsers
    - Safari - seems ok
    - FireFox (Mac) - seems ok
    - Chrome (Mac) - seems ok
    - FireFox (Win10) - seems ok
    - Chrome (Win10) - seems ok
    - Edge - seems ok
    - IE 11 - I'm going to give up on this one...
		- the add a link button dosn't insert a link in the right place
		- other things break periodically including:
			- the scroll position is not maintained while adding content with buttons
			- the sticky scroll toobar doesn't work in '_full height mode_'
- minor bugs
	- switching from visual to text mode doesn't maintain scroll position due to codemirror re-initalizing
 

## TODO later:
- add all these as enhancement requests
- add theme examples to screenshots
- store scroll position as well as cursor position
- support `<!--nextpage-->` in shortcode parser
- add fullscreen to plugin/theme editor
- success/progress/failure ui for saving options
- drag over line numbers to highlight lines
- [autoformat](http://codemirror.net/2/lib/util/formatting.js)? [demo](http://codemirror.net/2/demo/formatting.html) - this was discontinued
- addon/advanced options
	- keymaps
	- editor options:
		- style active line
		- matchBrackets
		- highlight selection matches
		- search
		- foldcode
	- code commands
		- commenting: Ctrl+/, Cmd+/
		- autoclose tags
		- autoclose brackets
		- [emmet](https://github.com/emmetio/codemirror)?
		- [spellcheck](https://github.com/NextStepWebs/codemirror-spell-checker)?
	- prevent reformatting like:
		- auto p
		- link to other auto p disabling plugins
- rtl support
- translation support
- IE & Edge Bug: adding content with the buttons doesn't work :(
	- ...because setting selection on a textarea doesn't work unless the text area is in focus
	- possible solution: 
		- detect mousedown on a button in the bar
		- give the real textarea focus and the proper selection
		- when that textarea changes, update the value in codemirror
		- then switch back to codemirror in the correct cursor position
- CodeMirror themes inspired by WordPress themes
	- and an auto theme that will match the CM theme to the WP theme - set by default
- compatible with other plugin:
	- [Site Origin Editor](https://siteorigin.com/widgets-bundle/)
	- [Advanced Custom Fields](https://www.advancedcustomfields.com/)
	- [Visual Composer](https://vc.wpbakery.com/)
	- [King Composer](https://wordpress.org/plugins/kingcomposer/)
	- [Revisionary](https://wordpress.org/plugins/revisionary/)
- read [bugs](https://wordpress.org/support/plugin/html-editor-syntax-highlighter) and add more TODOs


## Links
- process user settings
	- [working with user metadata](https://developer.wordpress.org/plugins/users/working-with-user-metadata/)
	- [update_user_meta()](https://codex.wordpress.org/Function_Reference/update_user_meta)
- AJAX forms
	- [submitting a form in wordpress using ajax](https://teamtreehouse.com/community/submitting-a-form-in-wordpress-using-ajax)
	- [how to handle form submission](http://wordpress.stackexchange.com/questions/60758/how-to-handle-form-submission)
- [wp usage stats](https://wordpress.org/about/stats/)


## Assets Info
[directions](https://developer.wordpress.org/plugins/wordpress-org/plugin-assets/)
- logos:
	- `assets/icon-128x128.png`
	- `assets/icon-256x256.png`
	- `assets/icon.svg`
- banner:
	- `assets/banner-1544x500.png`
	- `assets/banner-772x250.png`
	- `assets/banner-940x305.png`
	- `assets/banner-1880x610.png`
- screenshots: 
	- render at 1218px @ 2xDPI - 609px
	- [old style page](https://wordpress.org/plugins/html-editor-syntax-highlighter/screenshots/)
		- 902px(or less) wide @ <= 960px 
		- 543px wide @ < 960px
	- [new style page](https://wordpress.org/plugins-wp/html-editor-syntax-highlighter/)
		- 715px(or less) @ < 768px
		- 609px(or less) @ >= 768px
	- Syntax highlighting in the Post/Page HTML editor - `assets/screenshot-1.png`
	- Settings Panel - `assets/screenshot-2.png`
	- Syntax highlighting in the Theme/Plugin editor - `assets/screenshot-3.png`