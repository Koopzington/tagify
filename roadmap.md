- add SCSS variable for input color (not tag color)
- dragable sortable tags
- when "addTagOnBlur" is set to false and there is a text in the input and Tagify gets focus, the caret is not placed at the end of the input.
  (need to check if the "focus" event was fired programatically and if it, place the caret at the end)
- mix-mode: maybe convert "settings.pattern" to always be a regex. Currently it may be a String (this fails "validateTag" method)
- mix-mode: add "prefix" to tags, so when double-clicking to edit, it will show it
- maybe trigger the "invalid" event also for edited tags. need to think when exactly. probbaly not on "input" event, it's too much
- use DOM mutation to detect changes and update "this.value" automatically
- add examples of added tag CSS effects
- allow templates to return DOM nodes and not just Strings