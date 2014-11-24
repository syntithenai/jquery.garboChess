This plugin provides a user interface to play chess with move validation and optionally an AI to play against the computer.

garboChess.jquery is derived from https://github.com/glinscott/Garbochess-JS and has been modified to simplify and allow multiple use of the javascript in a single page.

Usual deal for installation
- requires jquery and jquery UI
- both garbochess.js and jquery.garbochess (in that order)
- access to img folder containing chess resources

$(document).ready(function () {
	$('.garbochess').garboChess();
});

The jquery plugin function can take the following options
styles - text chunk containing CSS rules
template - HTML to use for board rendering in none is provided as content of the jquery object
autoPlayDelay - delay before automatic move in ms. default 1000
showUI - UI components to make visible. default '.GameTitle,.board,.PgnTextBox,.NewGame,.UndoMove,.Suggest,.AutoMovesLabel'

The plugin triggers the following events
garbochess.Moved - when either a human or computer move is successfull and rendered  (for save)
garbochess.RedrawBoard - when the board is redrawn (for additional board UI binding)

