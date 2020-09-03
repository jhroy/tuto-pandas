<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />

<title>Tutoriel_pandas_en_francais</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>



<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.7.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.7.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff2?v=4.7.0') format('woff2'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.7.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.7.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.7.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.fa-pull-left {
  float: left;
}
.fa-pull-right {
  float: right;
}
.fa.fa-pull-left {
  margin-right: .3em;
}
.fa.fa-pull-right {
  margin-left: .3em;
}
/* Deprecated as of 4.4.0 */
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
.fa-pulse {
  -webkit-animation: fa-spin 1s infinite steps(8);
  animation: fa-spin 1s infinite steps(8);
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook-f:before,
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-feed:before,
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before,
.fa-gratipay:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper-pp:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-resistance:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-y-combinator-square:before,
.fa-yc-square:before,
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
.fa-buysellads:before {
  content: "\f20d";
}
.fa-connectdevelop:before {
  content: "\f20e";
}
.fa-dashcube:before {
  content: "\f210";
}
.fa-forumbee:before {
  content: "\f211";
}
.fa-leanpub:before {
  content: "\f212";
}
.fa-sellsy:before {
  content: "\f213";
}
.fa-shirtsinbulk:before {
  content: "\f214";
}
.fa-simplybuilt:before {
  content: "\f215";
}
.fa-skyatlas:before {
  content: "\f216";
}
.fa-cart-plus:before {
  content: "\f217";
}
.fa-cart-arrow-down:before {
  content: "\f218";
}
.fa-diamond:before {
  content: "\f219";
}
.fa-ship:before {
  content: "\f21a";
}
.fa-user-secret:before {
  content: "\f21b";
}
.fa-motorcycle:before {
  content: "\f21c";
}
.fa-street-view:before {
  content: "\f21d";
}
.fa-heartbeat:before {
  content: "\f21e";
}
.fa-venus:before {
  content: "\f221";
}
.fa-mars:before {
  content: "\f222";
}
.fa-mercury:before {
  content: "\f223";
}
.fa-intersex:before,
.fa-transgender:before {
  content: "\f224";
}
.fa-transgender-alt:before {
  content: "\f225";
}
.fa-venus-double:before {
  content: "\f226";
}
.fa-mars-double:before {
  content: "\f227";
}
.fa-venus-mars:before {
  content: "\f228";
}
.fa-mars-stroke:before {
  content: "\f229";
}
.fa-mars-stroke-v:before {
  content: "\f22a";
}
.fa-mars-stroke-h:before {
  content: "\f22b";
}
.fa-neuter:before {
  content: "\f22c";
}
.fa-genderless:before {
  content: "\f22d";
}
.fa-facebook-official:before {
  content: "\f230";
}
.fa-pinterest-p:before {
  content: "\f231";
}
.fa-whatsapp:before {
  content: "\f232";
}
.fa-server:before {
  content: "\f233";
}
.fa-user-plus:before {
  content: "\f234";
}
.fa-user-times:before {
  content: "\f235";
}
.fa-hotel:before,
.fa-bed:before {
  content: "\f236";
}
.fa-viacoin:before {
  content: "\f237";
}
.fa-train:before {
  content: "\f238";
}
.fa-subway:before {
  content: "\f239";
}
.fa-medium:before {
  content: "\f23a";
}
.fa-yc:before,
.fa-y-combinator:before {
  content: "\f23b";
}
.fa-optin-monster:before {
  content: "\f23c";
}
.fa-opencart:before {
  content: "\f23d";
}
.fa-expeditedssl:before {
  content: "\f23e";
}
.fa-battery-4:before,
.fa-battery:before,
.fa-battery-full:before {
  content: "\f240";
}
.fa-battery-3:before,
.fa-battery-three-quarters:before {
  content: "\f241";
}
.fa-battery-2:before,
.fa-battery-half:before {
  content: "\f242";
}
.fa-battery-1:before,
.fa-battery-quarter:before {
  content: "\f243";
}
.fa-battery-0:before,
.fa-battery-empty:before {
  content: "\f244";
}
.fa-mouse-pointer:before {
  content: "\f245";
}
.fa-i-cursor:before {
  content: "\f246";
}
.fa-object-group:before {
  content: "\f247";
}
.fa-object-ungroup:before {
  content: "\f248";
}
.fa-sticky-note:before {
  content: "\f249";
}
.fa-sticky-note-o:before {
  content: "\f24a";
}
.fa-cc-jcb:before {
  content: "\f24b";
}
.fa-cc-diners-club:before {
  content: "\f24c";
}
.fa-clone:before {
  content: "\f24d";
}
.fa-balance-scale:before {
  content: "\f24e";
}
.fa-hourglass-o:before {
  content: "\f250";
}
.fa-hourglass-1:before,
.fa-hourglass-start:before {
  content: "\f251";
}
.fa-hourglass-2:before,
.fa-hourglass-half:before {
  content: "\f252";
}
.fa-hourglass-3:before,
.fa-hourglass-end:before {
  content: "\f253";
}
.fa-hourglass:before {
  content: "\f254";
}
.fa-hand-grab-o:before,
.fa-hand-rock-o:before {
  content: "\f255";
}
.fa-hand-stop-o:before,
.fa-hand-paper-o:before {
  content: "\f256";
}
.fa-hand-scissors-o:before {
  content: "\f257";
}
.fa-hand-lizard-o:before {
  content: "\f258";
}
.fa-hand-spock-o:before {
  content: "\f259";
}
.fa-hand-pointer-o:before {
  content: "\f25a";
}
.fa-hand-peace-o:before {
  content: "\f25b";
}
.fa-trademark:before {
  content: "\f25c";
}
.fa-registered:before {
  content: "\f25d";
}
.fa-creative-commons:before {
  content: "\f25e";
}
.fa-gg:before {
  content: "\f260";
}
.fa-gg-circle:before {
  content: "\f261";
}
.fa-tripadvisor:before {
  content: "\f262";
}
.fa-odnoklassniki:before {
  content: "\f263";
}
.fa-odnoklassniki-square:before {
  content: "\f264";
}
.fa-get-pocket:before {
  content: "\f265";
}
.fa-wikipedia-w:before {
  content: "\f266";
}
.fa-safari:before {
  content: "\f267";
}
.fa-chrome:before {
  content: "\f268";
}
.fa-firefox:before {
  content: "\f269";
}
.fa-opera:before {
  content: "\f26a";
}
.fa-internet-explorer:before {
  content: "\f26b";
}
.fa-tv:before,
.fa-television:before {
  content: "\f26c";
}
.fa-contao:before {
  content: "\f26d";
}
.fa-500px:before {
  content: "\f26e";
}
.fa-amazon:before {
  content: "\f270";
}
.fa-calendar-plus-o:before {
  content: "\f271";
}
.fa-calendar-minus-o:before {
  content: "\f272";
}
.fa-calendar-times-o:before {
  content: "\f273";
}
.fa-calendar-check-o:before {
  content: "\f274";
}
.fa-industry:before {
  content: "\f275";
}
.fa-map-pin:before {
  content: "\f276";
}
.fa-map-signs:before {
  content: "\f277";
}
.fa-map-o:before {
  content: "\f278";
}
.fa-map:before {
  content: "\f279";
}
.fa-commenting:before {
  content: "\f27a";
}
.fa-commenting-o:before {
  content: "\f27b";
}
.fa-houzz:before {
  content: "\f27c";
}
.fa-vimeo:before {
  content: "\f27d";
}
.fa-black-tie:before {
  content: "\f27e";
}
.fa-fonticons:before {
  content: "\f280";
}
.fa-reddit-alien:before {
  content: "\f281";
}
.fa-edge:before {
  content: "\f282";
}
.fa-credit-card-alt:before {
  content: "\f283";
}
.fa-codiepie:before {
  content: "\f284";
}
.fa-modx:before {
  content: "\f285";
}
.fa-fort-awesome:before {
  content: "\f286";
}
.fa-usb:before {
  content: "\f287";
}
.fa-product-hunt:before {
  content: "\f288";
}
.fa-mixcloud:before {
  content: "\f289";
}
.fa-scribd:before {
  content: "\f28a";
}
.fa-pause-circle:before {
  content: "\f28b";
}
.fa-pause-circle-o:before {
  content: "\f28c";
}
.fa-stop-circle:before {
  content: "\f28d";
}
.fa-stop-circle-o:before {
  content: "\f28e";
}
.fa-shopping-bag:before {
  content: "\f290";
}
.fa-shopping-basket:before {
  content: "\f291";
}
.fa-hashtag:before {
  content: "\f292";
}
.fa-bluetooth:before {
  content: "\f293";
}
.fa-bluetooth-b:before {
  content: "\f294";
}
.fa-percent:before {
  content: "\f295";
}
.fa-gitlab:before {
  content: "\f296";
}
.fa-wpbeginner:before {
  content: "\f297";
}
.fa-wpforms:before {
  content: "\f298";
}
.fa-envira:before {
  content: "\f299";
}
.fa-universal-access:before {
  content: "\f29a";
}
.fa-wheelchair-alt:before {
  content: "\f29b";
}
.fa-question-circle-o:before {
  content: "\f29c";
}
.fa-blind:before {
  content: "\f29d";
}
.fa-audio-description:before {
  content: "\f29e";
}
.fa-volume-control-phone:before {
  content: "\f2a0";
}
.fa-braille:before {
  content: "\f2a1";
}
.fa-assistive-listening-systems:before {
  content: "\f2a2";
}
.fa-asl-interpreting:before,
.fa-american-sign-language-interpreting:before {
  content: "\f2a3";
}
.fa-deafness:before,
.fa-hard-of-hearing:before,
.fa-deaf:before {
  content: "\f2a4";
}
.fa-glide:before {
  content: "\f2a5";
}
.fa-glide-g:before {
  content: "\f2a6";
}
.fa-signing:before,
.fa-sign-language:before {
  content: "\f2a7";
}
.fa-low-vision:before {
  content: "\f2a8";
}
.fa-viadeo:before {
  content: "\f2a9";
}
.fa-viadeo-square:before {
  content: "\f2aa";
}
.fa-snapchat:before {
  content: "\f2ab";
}
.fa-snapchat-ghost:before {
  content: "\f2ac";
}
.fa-snapchat-square:before {
  content: "\f2ad";
}
.fa-pied-piper:before {
  content: "\f2ae";
}
.fa-first-order:before {
  content: "\f2b0";
}
.fa-yoast:before {
  content: "\f2b1";
}
.fa-themeisle:before {
  content: "\f2b2";
}
.fa-google-plus-circle:before,
.fa-google-plus-official:before {
  content: "\f2b3";
}
.fa-fa:before,
.fa-font-awesome:before {
  content: "\f2b4";
}
.fa-handshake-o:before {
  content: "\f2b5";
}
.fa-envelope-open:before {
  content: "\f2b6";
}
.fa-envelope-open-o:before {
  content: "\f2b7";
}
.fa-linode:before {
  content: "\f2b8";
}
.fa-address-book:before {
  content: "\f2b9";
}
.fa-address-book-o:before {
  content: "\f2ba";
}
.fa-vcard:before,
.fa-address-card:before {
  content: "\f2bb";
}
.fa-vcard-o:before,
.fa-address-card-o:before {
  content: "\f2bc";
}
.fa-user-circle:before {
  content: "\f2bd";
}
.fa-user-circle-o:before {
  content: "\f2be";
}
.fa-user-o:before {
  content: "\f2c0";
}
.fa-id-badge:before {
  content: "\f2c1";
}
.fa-drivers-license:before,
.fa-id-card:before {
  content: "\f2c2";
}
.fa-drivers-license-o:before,
.fa-id-card-o:before {
  content: "\f2c3";
}
.fa-quora:before {
  content: "\f2c4";
}
.fa-free-code-camp:before {
  content: "\f2c5";
}
.fa-telegram:before {
  content: "\f2c6";
}
.fa-thermometer-4:before,
.fa-thermometer:before,
.fa-thermometer-full:before {
  content: "\f2c7";
}
.fa-thermometer-3:before,
.fa-thermometer-three-quarters:before {
  content: "\f2c8";
}
.fa-thermometer-2:before,
.fa-thermometer-half:before {
  content: "\f2c9";
}
.fa-thermometer-1:before,
.fa-thermometer-quarter:before {
  content: "\f2ca";
}
.fa-thermometer-0:before,
.fa-thermometer-empty:before {
  content: "\f2cb";
}
.fa-shower:before {
  content: "\f2cc";
}
.fa-bathtub:before,
.fa-s15:before,
.fa-bath:before {
  content: "\f2cd";
}
.fa-podcast:before {
  content: "\f2ce";
}
.fa-window-maximize:before {
  content: "\f2d0";
}
.fa-window-minimize:before {
  content: "\f2d1";
}
.fa-window-restore:before {
  content: "\f2d2";
}
.fa-times-rectangle:before,
.fa-window-close:before {
  content: "\f2d3";
}
.fa-times-rectangle-o:before,
.fa-window-close-o:before {
  content: "\f2d4";
}
.fa-bandcamp:before {
  content: "\f2d5";
}
.fa-grav:before {
  content: "\f2d6";
}
.fa-etsy:before {
  content: "\f2d7";
}
.fa-imdb:before {
  content: "\f2d8";
}
.fa-ravelry:before {
  content: "\f2d9";
}
.fa-eercast:before {
  content: "\f2da";
}
.fa-microchip:before {
  content: "\f2db";
}
.fa-snowflake-o:before {
  content: "\f2dc";
}
.fa-superpowers:before {
  content: "\f2dd";
}
.fa-wpexplorer:before {
  content: "\f2de";
}
.fa-meetup:before {
  content: "\f2e0";
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
div.traceback-wrapper pre.traceback {
  max-height: 600px;
  overflow: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 5px;
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
[dir="rtl"] #ipython_notebook {
  margin-right: 10px;
  margin-left: 0;
}
[dir="rtl"] #ipython_notebook.pull-left {
  float: right !important;
  float: right;
}
.flex-spacer {
  flex: 1;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#kernel_logo_widget {
  margin: 0 10px;
}
span#login_widget {
  float: right;
}
[dir="rtl"] span#login_widget {
  float: left;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
.modal-header {
  cursor: move;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
[dir="rtl"] .center-nav form.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] .center-nav .navbar-text {
  float: right;
}
[dir="rtl"] .navbar-inner {
  text-align: right;
}
[dir="rtl"] div.text-left {
  text-align: right;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  overflow: hidden;
  cursor: pointer;
  opacity: 0;
  z-index: 2;
}
.alternate_upload .btn-xs > input.fileinput {
  margin: -1px -5px;
}
.alternate_upload .btn-upload {
  position: relative;
  height: 22px;
}
::-webkit-file-upload-button {
  cursor: pointer;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
ul#tabs {
  margin-bottom: 4px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
[dir="rtl"] ul#tabs.nav-tabs > li {
  float: right;
}
[dir="rtl"] ul#tabs.nav.nav-tabs {
  padding-right: 0;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons .pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .list_toolbar .col-sm-4,
[dir="rtl"] .list_toolbar .col-sm-8 {
  float: right;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: text-bottom;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
[dir="rtl"] .list_item > div input {
  margin-right: 0;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_modified {
  margin-right: 7px;
  margin-left: 7px;
}
[dir="rtl"] .item_modified.pull-right {
  float: left !important;
  float: left;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
[dir="rtl"] .item_buttons.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .item_buttons .kernel-name {
  margin-left: 7px;
  float: right;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
.sort_button {
  display: inline-block;
  padding-left: 7px;
}
[dir="rtl"] .sort_button.pull-right {
  float: left !important;
  float: left;
}
#tree-selector {
  padding-right: 0px;
}
#button-select-all {
  min-width: 50px;
}
[dir="rtl"] #button-select-all.btn {
  float: right ;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
  margin-top: 2px;
  height: 16px;
}
[dir="rtl"] #select-all.pull-left {
  float: right !important;
  float: right;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.fa-pull-left {
  margin-right: .3em;
}
.folder_icon:before.fa-pull-right {
  margin-left: .3em;
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.fa-pull-left {
  margin-right: .3em;
}
.file_icon:before.fa-pull-right {
  margin-left: .3em;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
#new-menu .dropdown-header {
  font-size: 10px;
  border-bottom: 1px solid #e5e5e5;
  padding: 0 0 3px;
  margin: -3px 20px 0;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.move-button {
  display: none;
}
.download-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
.CodeMirror-dialog {
  background-color: #fff;
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI escape sequences */
/* The color values are a mix of
   http://www.xcolors.net/dl/baskerville-ivorylight and
   http://www.xcolors.net/dl/euphrasia */
.ansi-black-fg {
  color: #3E424D;
}
.ansi-black-bg {
  background-color: #3E424D;
}
.ansi-black-intense-fg {
  color: #282C36;
}
.ansi-black-intense-bg {
  background-color: #282C36;
}
.ansi-red-fg {
  color: #E75C58;
}
.ansi-red-bg {
  background-color: #E75C58;
}
.ansi-red-intense-fg {
  color: #B22B31;
}
.ansi-red-intense-bg {
  background-color: #B22B31;
}
.ansi-green-fg {
  color: #00A250;
}
.ansi-green-bg {
  background-color: #00A250;
}
.ansi-green-intense-fg {
  color: #007427;
}
.ansi-green-intense-bg {
  background-color: #007427;
}
.ansi-yellow-fg {
  color: #DDB62B;
}
.ansi-yellow-bg {
  background-color: #DDB62B;
}
.ansi-yellow-intense-fg {
  color: #B27D12;
}
.ansi-yellow-intense-bg {
  background-color: #B27D12;
}
.ansi-blue-fg {
  color: #208FFB;
}
.ansi-blue-bg {
  background-color: #208FFB;
}
.ansi-blue-intense-fg {
  color: #0065CA;
}
.ansi-blue-intense-bg {
  background-color: #0065CA;
}
.ansi-magenta-fg {
  color: #D160C4;
}
.ansi-magenta-bg {
  background-color: #D160C4;
}
.ansi-magenta-intense-fg {
  color: #A03196;
}
.ansi-magenta-intense-bg {
  background-color: #A03196;
}
.ansi-cyan-fg {
  color: #60C6C8;
}
.ansi-cyan-bg {
  background-color: #60C6C8;
}
.ansi-cyan-intense-fg {
  color: #258F8F;
}
.ansi-cyan-intense-bg {
  background-color: #258F8F;
}
.ansi-white-fg {
  color: #C5C1B4;
}
.ansi-white-bg {
  background-color: #C5C1B4;
}
.ansi-white-intense-fg {
  color: #A1A6B2;
}
.ansi-white-intense-bg {
  background-color: #A1A6B2;
}
.ansi-default-inverse-fg {
  color: #FFFFFF;
}
.ansi-default-inverse-bg {
  background-color: #000000;
}
.ansi-bold {
  font-weight: bold;
}
.ansi-underline {
  text-decoration: underline;
}
/* The following styles are deprecated an will be removed in a future version */
.ansibold {
  font-weight: bold;
}
.ansi-inverse {
  outline: 0.5px dotted;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  position: relative;
  overflow: visible;
}
div.cell:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: transparent;
}
div.cell.jupyter-soft-selected {
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected,
div.cell.selected.jupyter-soft-selected {
  border-color: #ababab;
}
div.cell.selected:before,
div.cell.selected.jupyter-soft-selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #42A5F5;
}
@media print {
  div.cell.selected,
  div.cell.selected.jupyter-soft-selected {
    border-color: transparent;
  }
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
}
.edit_mode div.cell.selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #66BB6A;
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  /* Note that this should set vertical padding only, since CodeMirror assumes
       that horizontal padding will be set on CodeMirror pre */
  padding: 0.4em 0;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. This sets horizontal padding only,
    use .CodeMirror-lines for vertical */
  padding: 0 0.4em;
  border: 0;
  border-radius: 0;
}
.CodeMirror-cursor {
  border-left: 1.4px solid black;
}
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor {
    border-left: 2px solid black;
  }
}
@media screen and (min-width: 4320px) {
  .CodeMirror-cursor {
    border-left: 4px solid black;
  }
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
div.output_area .mglyph > img {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 1px 0 1px 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul:not(.list-inline),
.rendered_html ol:not(.list-inline) {
  padding-left: 2em;
}
.rendered_html ul {
  list-style: disc;
}
.rendered_html ul ul {
  list-style: square;
  margin-top: 0;
}
.rendered_html ul ul ul {
  list-style: circle;
}
.rendered_html ol {
  list-style: decimal;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin-top: 0;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
  padding: 0px;
  background-color: #fff;
}
.rendered_html code {
  background-color: #eff0f1;
}
.rendered_html p code {
  padding: 1px 5px;
}
.rendered_html pre code {
  background-color: #fff;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  color: #000;
  font-size: 100%;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: none;
  border-collapse: collapse;
  border-spacing: 0;
  color: black;
  font-size: 12px;
  table-layout: fixed;
}
.rendered_html thead {
  border-bottom: 1px solid black;
  vertical-align: bottom;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  text-align: right;
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html tbody tr:nth-child(odd) {
  background: #f5f5f5;
}
.rendered_html tbody tr:hover {
  background: rgba(66, 165, 245, 0.2);
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
.rendered_html .alert {
  margin-bottom: initial;
}
.rendered_html * + .alert {
  margin-top: 1em;
}
[dir="rtl"] .rendered_html p {
  text-align: right;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.rendered .rendered_html tr,
.text_cell.rendered .rendered_html th,
.text_cell.rendered .rendered_html td {
  max-width: none;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.text_cell .dropzone .input_area {
  border: 2px dashed #bababa;
  margin: -1px;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
.jupyter-keybindings {
  padding: 1px;
  line-height: 24px;
  border-bottom: 1px solid gray;
}
.jupyter-keybindings input {
  margin: 0;
  padding: 0;
  border: none;
}
.jupyter-keybindings i {
  padding: 6px;
}
.well code {
  background-color: #ffffff;
  border-color: #ababab;
  border-width: 1px;
  border-style: solid;
  padding: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.tags_button_container {
  width: 100%;
  display: flex;
}
.tag-container {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  overflow: hidden;
  position: relative;
}
.tag-container > * {
  margin: 0 4px;
}
.remove-tag-btn {
  margin-left: 4px;
}
.tags-input {
  display: flex;
}
.cell-tag:last-child:after {
  content: "";
  position: absolute;
  right: 0;
  width: 40px;
  height: 100%;
  /* Fade to background color of cell toolbar */
  background: linear-gradient(to right, rgba(0, 0, 0, 0), #EEE);
}
.tags-input > * {
  margin-left: 4px;
}
.cell-tag,
.tags-input input,
.tags-input button {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  box-shadow: none;
  width: inherit;
  font-size: inherit;
  height: 22px;
  line-height: 22px;
  padding: 0px 4px;
  display: inline-block;
}
.cell-tag:focus,
.tags-input input:focus,
.tags-input button:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.cell-tag::-moz-placeholder,
.tags-input input::-moz-placeholder,
.tags-input button::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.cell-tag:-ms-input-placeholder,
.tags-input input:-ms-input-placeholder,
.tags-input button:-ms-input-placeholder {
  color: #999;
}
.cell-tag::-webkit-input-placeholder,
.tags-input input::-webkit-input-placeholder,
.tags-input button::-webkit-input-placeholder {
  color: #999;
}
.cell-tag::-ms-expand,
.tags-input input::-ms-expand,
.tags-input button::-ms-expand {
  border: 0;
  background-color: transparent;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
.cell-tag[readonly],
.tags-input input[readonly],
.tags-input button[readonly],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  background-color: #eeeeee;
  opacity: 1;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  cursor: not-allowed;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button {
  height: auto;
}
select.cell-tag,
select.tags-input input,
select.tags-input button {
  height: 30px;
  line-height: 30px;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button,
select[multiple].cell-tag,
select[multiple].tags-input input,
select[multiple].tags-input button {
  height: auto;
}
.cell-tag,
.tags-input button {
  padding: 0px 4px;
}
.cell-tag {
  background-color: #fff;
  white-space: nowrap;
}
.tags-input input[type=text]:focus {
  outline: none;
  box-shadow: none;
  border-color: #ccc;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
[dir="rtl"] #kernel_logo_widget {
  float: left !important;
  float: left;
}
.modal .modal-body .move-path {
  display: flex;
  flex-direction: row;
  justify-content: space;
  align-items: center;
}
.modal .modal-body .move-path .server-root {
  padding-right: 20px;
}
.modal .modal-body .move-path .path-input {
  flex: 1;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
[dir="rtl"] #menubar .navbar-toggle {
  float: right;
}
[dir="rtl"] #menubar .navbar-collapse {
  clear: right;
}
[dir="rtl"] #menubar .navbar-nav {
  float: right;
}
[dir="rtl"] #menubar .nav {
  padding-right: 0px;
}
[dir="rtl"] #menubar .navbar-nav > li {
  float: right;
}
[dir="rtl"] #menubar .navbar-right {
  float: left !important;
}
[dir="rtl"] ul.dropdown-menu {
  text-align: right;
  left: auto;
}
[dir="rtl"] ul#new-menu.dropdown-menu {
  right: auto;
  left: 0;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
[dir="rtl"] i.menu-icon.pull-right {
  float: left !important;
  float: left;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
[dir="rtl"] ul#help_menu li a {
  padding-left: 2.2em;
}
[dir="rtl"] ul#help_menu li a i {
  margin-right: 0;
  margin-left: -1.2em;
}
[dir="rtl"] ul#help_menu li a i.pull-right {
  float: left !important;
  float: left;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
[dir="rtl"] .dropdown-submenu > .dropdown-menu {
  right: 100%;
  margin-right: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.fa-pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.fa-pull-right {
  margin-left: .3em;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
[dir="rtl"] .dropdown-submenu > a:after {
  float: left;
  content: "\f0d9";
  margin-right: 0;
  margin-left: -10px;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
[dir="rtl"] #notification_area {
  float: left !important;
  float: left;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] .indicator_area {
  float: left !important;
  float: left;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
[dir="rtl"] #kernel_indicator {
  float: left !important;
  float: left;
  border-left: 0;
  border-right: 1px solid;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] #modal_indicator {
  float: left !important;
  float: left;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  height: 30px;
  margin-top: 4px;
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  width: 50%;
  flex: 1;
}
span.save_widget span.filename {
  height: 100%;
  line-height: 1em;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
[dir="rtl"] span.save_widget.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] span.save_widget span.filename {
  margin-left: 0;
  margin-right: 16px;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
  white-space: nowrap;
  padding: 0 5px;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
    padding: 0 0 0 5px;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
.toolbar-btn-label {
  margin-left: 6px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
[dir="rtl"] .btn-group > .btn,
.btn-group-vertical > .btn {
  float: right;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
[dir="rtl"] ul.typeahead-list i {
  margin-left: 0;
  margin-right: -10px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
ul.typeahead-list  > li > a.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .typeahead-list {
  text-align: right;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  min-width: 20px;
  color: transparent;
}
[dir="rtl"] .no-shortcut.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .command-shortcut.pull-right {
  float: left !important;
  float: left;
}
.command-shortcut:before {
  content: "(command mode)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
[dir="rtl"] .edit-shortcut.pull-right {
  float: left !important;
  float: left;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
[dir="ltr"] #find-and-replace .input-group-btn + .form-control {
  border-left: none;
}
[dir="rtl"] #find-and-replace .input-group-btn + .form-control {
  border-right: none;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Introduction-&#224;-pandas">Introduction &#224; pandas<a class="anchor-link" href="#Introduction-&#224;-pandas">&#182;</a></h1><h3 id="Ou-comment-devenir-un-ninja-des-donn&#233;es">Ou comment devenir un ninja des donn&#233;es<a class="anchor-link" href="#Ou-comment-devenir-un-ninja-des-donn&#233;es">&#182;</a></h3><hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><img src="https://pandas.pydata.org/docs/_static/pandas.svg" alt="Logo de pandas">
Tutoriel sur <a href="http://pandas.pydata.org/">pandas</a> (<a href="http://pandas.pydata.org/pandas-docs/stable/index.html">documentation</a>), bibliothèque python permettant d'analyser et d'interroger rapidement des données; particulièrement utile lorsqu'on a des fichiers volumineux qu'un tableur comme <em>Excel</em>, <em>Calc</em> ou <em>Google Sheets</em> a de la difficulté à avaler. Contenu préparé pour le <a href="https://www.gitbook.com/book/jhroy/edm5240-h2017/details">EDM5240</a>, cours de journalisme informatique de l'<a href="http://uqam.ca/">Université du Québec à Montréal</a> (mars 2017; mis à jour en mars 2019), plus récemment changé pour <a href="https://journalisme-uqam.gitbook.io/edm4466-h2020/">EDM4466 (Journalisme de données II)</a>.<br></p>
<hr>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Le premier bloc de code, ci-dessous, ressemble au début des scripts que vous avez réalisés jusqu'à maintenant. Il s'agit d'importer les modules dont nous aurons besoin. On leur donne même un surnom. C'est ainsi que <strong><code>pandas</code></strong> devient <strong><code>pd</code></strong>, par exemple.
<br>
La ligne <strong><code>%matplotlib inline</code></strong> sert simplement à demander à notre carnet d'afficher des graphiques dans la page lorsqu'on souhaitera en créer.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="o">%</span><span class="k">matplotlib</span> inline
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">matplotlib</span> <span class="k">as</span> <span class="nn">mp</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut changer les options d'affichage de pandas avec la fonction <code>.set_option</code>.<br>
Ici, on demande que l'affichage des nombres ne soit <strong>pas</strong> en notation scientifique, comme il l'est par défaut.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">pd</span><span class="o">.</span><span class="n">options</span><span class="o">.</span><span class="n">display</span><span class="o">.</span><span class="n">float_format</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="si">{:.2f}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ci-dessous, on lit <a href="http://bit.ly/jhroypandas">deux des fichiers que je vous ai donnés</a>.<br>
On les mets chacun dans une variable. J'ai choisi de baptiser l'une de ces variables <code>md</code> puisque le fichier indiqué comprend des données sur l'ensemble des membres du Collège des médecins, et l'autre <code>mil</code> puisque le fichier indiqué contient, pour sa part, des données sur les contrats octroyés par le ministère de la Défense nationale.<br>
Pour pandas, cette structure de données, qui consiste en un tableau à deux dimensions, est appelé un <em><strong>dataframe</strong></em>.<br></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="s2">&quot;cmq.csv&quot;</span><span class="p">)</span>
<span class="n">mil</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="s2">&quot;militaires.csv&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour connaître le type des variables que contient notre tableau, on peut utiliser la fonction <code>.dtypes</code>.<p>
Dans pandas, les principaux types de variables sont&nbsp;:</p>
<ul>
<li><code>int</code> -&gt; nombres entiers</li>
<li><code>float</code> -&gt; nombres décimaux</li>
<li><code>object</code> -&gt; chaînes de caractères</li>
<li><code>datetime</code> -&gt; dates</li>
<li><code>bool</code> -&gt; vrai ou faux</li>
</ul>
<p>Ces types sont parfois suivis d'un nombre qui indique la taille, en caractères, maximale des variables de ce type.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">dtypes</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[4]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>num                object
annee               int64
prenom             object
nom                object
genre              object
specialite1        object
specialite2        object
specialite3        object
statut             object
dateChangStatut    object
typePermis         object
ville              object
prov               object
pays               object
dtype: object</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">dtypes</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[5]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>annee            int64
trimestre        int64
date            object
fournisseur     object
description     object
montant        float64
dtype: object</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Exploration-simple-de-nos-donn&#233;es">Exploration simple de nos donn&#233;es<a class="anchor-link" href="#Exploration-simple-de-nos-donn&#233;es">&#182;</a></h2><hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour afficher simplement le contenu de notre variable, il n'est pas nécessaire d'écrire <code>print(md)</code>.<br>Écrire le nom de la variable suffit.<br>
Cela produit un immense tableau avec les 30 premières et les 30 dernières lignes de notre fichier.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[6]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>#30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>#30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Alma</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>#30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>#30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>#30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>#16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>#16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>#16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>#16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>#16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>35109 rows × 14 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour avoir un aperçu des dimensions de de votre tableau, utilisez plutôt la fonction <code>.shape</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">shape</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[7]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>(35109, 14)</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour consulter les premières ou les dernières lignes de votre tableau, vous pouvez vous servir de fonctions qui ressemblent à ce qu'on a vu dans <a href="http://bit.ly/jhroyunix">Unix</a>, au début de la session, <code>.head()</code> et <code>.tail()</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[8]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>#30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>#30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Alma</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>#30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>#30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>#30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">tail</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[9]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>annee</th>
      <th>trimestre</th>
      <th>date</th>
      <th>fournisseur</th>
      <th>description</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>165947</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>NB Harrison Inc</td>
      <td>Opérations de parachutage</td>
      <td>30700.00</td>
    </tr>
    <tr>
      <th>165948</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>Clint Clawson</td>
      <td>Opérations de parachutage</td>
      <td>41250.00</td>
    </tr>
    <tr>
      <th>165949</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>The Goodyear Tire &amp; Rubber Company</td>
      <td>Pneumatiques et chambres à air d'aéronefs</td>
      <td>282000.00</td>
    </tr>
    <tr>
      <th>165950</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>Imperial Oil Limited</td>
      <td>Combustible d'aviation</td>
      <td>315315.20</td>
    </tr>
    <tr>
      <th>165951</th>
      <td>2016</td>
      <td>3</td>
      <td>30-12-2016</td>
      <td>S.M.I. Support Measures Inc.</td>
      <td>Antennes, guides d'ondes et équipement connexe...</td>
      <td>630000.00</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour consulter un intervalle précis de lignes, vous pouvez vous servir des crochets. Vous reconnaissez cette syntaxe puisque pandas, c'est du python!<br>
C'est ainsi que, ci-dessous, je demande à afficher les lignes 1000 à 1009 de mon fichier (comme en python, la limite supérieure est exclue de mon intervalle).</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="mi">1000</span><span class="p">:</span><span class="mi">1010</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[10]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>dateChangStatut</th>
      <th>typePermis</th>
      <th>ville</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1000</th>
      <td>#44048</td>
      <td>1944</td>
      <td>Paul H.</td>
      <td>Niloff</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1992-02-12</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1001</th>
      <td>#44049</td>
      <td>1944</td>
      <td>Walter C.</td>
      <td>Lloyd-Smith</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1999-07-01</td>
      <td>Régulier</td>
      <td>Sillery</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1002</th>
      <td>#44050</td>
      <td>1944</td>
      <td>Jean-Benoit</td>
      <td>Bechard</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2008-05-02</td>
      <td>Régulier</td>
      <td>Saint-Lambert</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1003</th>
      <td>#44051</td>
      <td>1944</td>
      <td>H. F.</td>
      <td>Brickman</td>
      <td>F</td>
      <td>Pédiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié pour non-paiement de cotisation</td>
      <td>1964-08-31</td>
      <td>Régulier</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inconnu</td>
    </tr>
    <tr>
      <th>1004</th>
      <td>#44052</td>
      <td>1944</td>
      <td>E. R.</td>
      <td>Mackenzie-Harpur</td>
      <td>F</td>
      <td>Biochimie médicale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2001-02-18</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1005</th>
      <td>#44054</td>
      <td>1944</td>
      <td>Claude</td>
      <td>Dubé</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1982-09-22</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1006</th>
      <td>#44055</td>
      <td>1944</td>
      <td>Alban</td>
      <td>Damphousse</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-11-03</td>
      <td>Régulier</td>
      <td>Montréal</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1007</th>
      <td>#44056</td>
      <td>1944</td>
      <td>James L.</td>
      <td>Mc Callum</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1999-04-12</td>
      <td>Régulier</td>
      <td>Bellefeuille</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1008</th>
      <td>#44057</td>
      <td>1944</td>
      <td>Samuel A.</td>
      <td>Macdonald</td>
      <td>M</td>
      <td>Urologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1995-04-02</td>
      <td>Régulier</td>
      <td>Saint-Laurent</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1009</th>
      <td>#44061</td>
      <td>1944</td>
      <td>Léon</td>
      <td>Leclerc</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-09-30</td>
      <td>Régulier</td>
      <td>Sillery</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Pour faire afficher un nombre limité de colonnes, on peut ajouter une liste du nom des colonnes qu'on souhaite.<br>
Il faut cependant le faire avec la fonction <code>.loc</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="mi">7000</span><span class="p">:</span><span class="mi">7010</span><span class="p">,[</span><span class="s2">&quot;nom&quot;</span><span class="p">,</span><span class="s2">&quot;prenom&quot;</span><span class="p">,</span><span class="s2">&quot;num&quot;</span><span class="p">]]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[11]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>nom</th>
      <th>prenom</th>
      <th>num</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>7000</th>
      <td>Behroozi</td>
      <td>Cyrus</td>
      <td>#67360</td>
    </tr>
    <tr>
      <th>7001</th>
      <td>Diez</td>
      <td>Garcia Pablo</td>
      <td>#67361</td>
    </tr>
    <tr>
      <th>7002</th>
      <td>Coles</td>
      <td>Duval</td>
      <td>#67362</td>
    </tr>
    <tr>
      <th>7003</th>
      <td>Pritchard</td>
      <td>Élizabeth</td>
      <td>#67363</td>
    </tr>
    <tr>
      <th>7004</th>
      <td>Braithwaite</td>
      <td>Desmond</td>
      <td>#67364</td>
    </tr>
    <tr>
      <th>7005</th>
      <td>Freeman</td>
      <td>Lincoln C.</td>
      <td>#67365</td>
    </tr>
    <tr>
      <th>7006</th>
      <td>Murat</td>
      <td>Paul</td>
      <td>#67366</td>
    </tr>
    <tr>
      <th>7007</th>
      <td>Khoury-Haddad</td>
      <td>Albert</td>
      <td>#67367</td>
    </tr>
    <tr>
      <th>7008</th>
      <td>Clecner</td>
      <td>Bya</td>
      <td>#67368</td>
    </tr>
    <tr>
      <th>7009</th>
      <td>Papapetropoulos</td>
      <td>D.</td>
      <td>#67369</td>
    </tr>
    <tr>
      <th>7010</th>
      <td>Gabriel</td>
      <td>Chafik N.</td>
      <td>#67370</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut aussi utiliser, au lieu du nom des colonnes, le numéro d'index des colonnes qu'on souhaite afficher.<br>
Il faut alors utiliser la fonction <code>.iloc</code></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">iloc</span><span class="p">[</span><span class="mi">100000</span><span class="p">:</span><span class="mi">100011</span><span class="p">,</span><span class="mi">3</span><span class="p">:]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[12]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>fournisseur</th>
      <th>description</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>100000</th>
      <td>MLS USA Corporation</td>
      <td>Articles divers (Comprend seulement ces articl...</td>
      <td>158732.13</td>
    </tr>
    <tr>
      <th>100001</th>
      <td>Turtle Island Staffing</td>
      <td>Services d'aide temporaire, soutien administra...</td>
      <td>46782.00</td>
    </tr>
    <tr>
      <th>100002</th>
      <td>IMPERIAL OIL</td>
      <td>MAZOUT</td>
      <td>14329.30</td>
    </tr>
    <tr>
      <th>100003</th>
      <td>IMPERIAL OIL</td>
      <td>MAZOUT</td>
      <td>14663.55</td>
    </tr>
    <tr>
      <th>100004</th>
      <td>Valley Refrigeration Limited</td>
      <td>Travaux professionnels spéciaux de construction</td>
      <td>73989.47</td>
    </tr>
    <tr>
      <th>100005</th>
      <td>Centaur Products inc.</td>
      <td>Travaux de construction pour édifices</td>
      <td>74294.00</td>
    </tr>
    <tr>
      <th>100006</th>
      <td>Tayco Paving Company</td>
      <td>Travaux de construction - génie civil</td>
      <td>195725.00</td>
    </tr>
    <tr>
      <th>100007</th>
      <td>MCM Architects Inc.</td>
      <td>Services d'architecture et d'ingénierie - Cons...</td>
      <td>71851.00</td>
    </tr>
    <tr>
      <th>100008</th>
      <td>Shamrock Building Services Ltd</td>
      <td>Travaux de construction pour édifices</td>
      <td>168400.00</td>
    </tr>
    <tr>
      <th>100009</th>
      <td>SNC-Lavalin Environment Inc.  (Victoria)</td>
      <td>Services environnementaux</td>
      <td>71765.00</td>
    </tr>
    <tr>
      <th>100010</th>
      <td>LVM Inc.   (Montreal)</td>
      <td>Services environnementaux</td>
      <td>13731.94</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Si on souhaite compter combien il y a d'éléments dans chacune de nos colonnes, on peut utiliser la fonction <code>.count()</code>.<br>
Employons-la avec nos deux fichiers.</p>
<p>On constate qu'avec les médecins, il nous manque parfois de l'information. Cela peut faire du sens, comme pour les colonnes <code>specialite2</code> et <code>specialite3</code>, puisque ce ne sont pas tous les médecins qui ont deux ou trois spécialités. Mais cela peut aussi vouloir dire qu'il y a des données manquantes. Ainsi, on n'a pas la ville dans laquelle excercent tous les médecins.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[13]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">count</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[13]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>num                35109
annee              35109
prenom             35108
nom                35109
genre              35109
specialite1        35109
specialite2         3467
specialite3          224
statut             35109
dateChangStatut    11412
typePermis         35109
ville              33715
prov               34133
pays               35109
dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[14]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">count</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[14]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>annee          165952
trimestre      165952
date           165952
fournisseur    165952
description    165945
montant        165952
dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Op&#233;rations-sur-les-colonnes">Op&#233;rations sur les colonnes<a class="anchor-link" href="#Op&#233;rations-sur-les-colonnes">&#182;</a></h2><hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il est souvent utile de connaître le nom des colonnes de notre fichier.<br>
Pour ce faire, entrez la fonction <code>.columns</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[15]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">columns</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[15]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Index([&#39;num&#39;, &#39;annee&#39;, &#39;prenom&#39;, &#39;nom&#39;, &#39;genre&#39;, &#39;specialite1&#39;, &#39;specialite2&#39;,
       &#39;specialite3&#39;, &#39;statut&#39;, &#39;dateChangStatut&#39;, &#39;typePermis&#39;, &#39;ville&#39;,
       &#39;prov&#39;, &#39;pays&#39;],
      dtype=&#39;object&#39;)</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Vous remarquez que le nom de chaque colonne se trouve dans une liste. On peut se servir de cette liste pour renommer nos colonnes dans le cas où elles ont des noms barbares. Il suffit de dire que <code>md.columns</code> est égal à une liste dans laquelle on mettra nos nouveaux noms de colonnes.<br>
C'est ainsi que la commande ci-dessous, par exemple, me permet de rebaptiser la colonne <code>dateChangStatut</code> par <code>date</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[16]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;num&#39;</span><span class="p">,</span> <span class="s1">&#39;annee&#39;</span><span class="p">,</span> <span class="s1">&#39;prenom&#39;</span><span class="p">,</span> <span class="s1">&#39;nom&#39;</span><span class="p">,</span> <span class="s1">&#39;genre&#39;</span><span class="p">,</span> <span class="s1">&#39;specialite1&#39;</span><span class="p">,</span> <span class="s1">&#39;specialite2&#39;</span><span class="p">,</span>
       <span class="s1">&#39;specialite3&#39;</span><span class="p">,</span> <span class="s1">&#39;statut&#39;</span><span class="p">,</span> <span class="s1">&#39;date&#39;</span><span class="p">,</span> <span class="s1">&#39;typePermis&#39;</span><span class="p">,</span> <span class="s1">&#39;ville&#39;</span><span class="p">,</span>
       <span class="s1">&#39;prov&#39;</span><span class="p">,</span> <span class="s1">&#39;pays&#39;</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>En invoquant la fonction <code>.columns</code>, je constate que le nom de la colonne a changé.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[17]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">columns</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[17]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Index([&#39;num&#39;, &#39;annee&#39;, &#39;prenom&#39;, &#39;nom&#39;, &#39;genre&#39;, &#39;specialite1&#39;, &#39;specialite2&#39;,
       &#39;specialite3&#39;, &#39;statut&#39;, &#39;date&#39;, &#39;typePermis&#39;, &#39;ville&#39;, &#39;prov&#39;, &#39;pays&#39;],
      dtype=&#39;object&#39;)</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ce n'est pas le cas ici, mais il arrive fréquemment, lorsqu'on travaille avec des données ouvertes, qu'il y a beaucoup de colonnes. Cela peut rendre les données difficiles à lire, sans compter que ça peut taxer la mémoire de notre ordi. Il est possible de supprimer des colonnes contenant des informations superflues.</p>
<p>Si, par exemple, dans le fichier de médecins, vous souhaitiez vous débarasser de la colonne <code>ville</code>, ce serait avec la fonction <code>.drop()</code> que vous vous y prendriez.</p>
<p>Cette fonction prend deux arguments. Le premier est la colonne (ou les colonnes) que vous souhaitez rayer de la surface de la Terre. Lorsqu'il y a plusieurs colonnes, il faut les mettre dans une liste&nbsp;: <code>["colonne_1", "colonne_2", "colonne_3"]</code>. Le second indique si ce sont des colonnes que vous souhaitez supprimer ou des lignes. Dans le cas de colonnes, l'argument doit être <code>1</code>, dans le cas de lignes, c'est <code>0</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[18]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="s2">&quot;ville&quot;</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[19]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">columns</span> <span class="c1"># La colonne «ville» a disparu!</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[19]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Index([&#39;num&#39;, &#39;annee&#39;, &#39;prenom&#39;, &#39;nom&#39;, &#39;genre&#39;, &#39;specialite1&#39;, &#39;specialite2&#39;,
       &#39;specialite3&#39;, &#39;statut&#39;, &#39;date&#39;, &#39;typePermis&#39;, &#39;prov&#39;, &#39;pays&#39;],
      dtype=&#39;object&#39;)</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il est utile de simplifier les noms des colonnes puisqu'on peut faire afficher le contenu d'une colonne de notre choix simplement en ajoutant son nom à notre nom de variable.<br>
On obtient alors non plus un <em><strong>dataframe</strong></em>, mais une structure de données unidimentionnelle que pandas appelle une <em><strong>serie</strong></em>.</p>
<p>Voici un exemple avec le genre des médecins&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[20]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">genre</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[20]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0        M
1        M
2        M
3        M
4        M
        ..
35104    M
35105    M
35106    F
35107    F
35108    M
Name: genre, Length: 35109, dtype: object</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Op&#233;rations-de-base">Op&#233;rations de base<a class="anchor-link" href="#Op&#233;rations-de-base">&#182;</a></h2><hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Cette sélection de colonnes est utile pour effectuer une série d'opérations de base qu'on va maintenant aborder.<br>
Si on a une colonne qui contient des nombres, on peut en afficher la valeur maximale ou minimale à l'aide des fonctions <code>.max()</code> et <code>.min()</code>.<br>
Voici un exemple avec la colonne <code>montant</code> de notre fichier de données sur les contrats militaires.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[21]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">max</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[21]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>9975000.0</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[22]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">min</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[22]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0.0</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut aussi effectuer des calculs simples sur ces colonnes.<br>
Ici, on effectue :</p>
<ul>
<li>une somme avec la fonction <code>.sum()</code></li>
<li>une moyenne avec la fonction <code>.mean()</code></li>
</ul>
<p>Et on trouve la médiane avec la fonction <code>.median()</code></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[23]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>27163294776.26</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">mean</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[24]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>163681.63551063047</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">median</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[25]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>28984.5</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Dans les cas où vous avez plusieurs colonnes composées de nombres, il peut être intéressant de réunir toutes ces informations à l'intérieur d'un seul et même tableau.<br>
C'est ce que nous permet de faire la fonction <code>.describe()</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[26]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[26]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>annee</th>
      <th>trimestre</th>
      <th>montant</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>165952.00</td>
      <td>165952.00</td>
      <td>165952.00</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>2010.87</td>
      <td>2.57</td>
      <td>163681.64</td>
    </tr>
    <tr>
      <th>std</th>
      <td>3.27</td>
      <td>1.11</td>
      <td>595860.66</td>
    </tr>
    <tr>
      <th>min</th>
      <td>2004.00</td>
      <td>1.00</td>
      <td>0.00</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2009.00</td>
      <td>2.00</td>
      <td>15754.75</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>2011.00</td>
      <td>3.00</td>
      <td>28984.50</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>2014.00</td>
      <td>4.00</td>
      <td>86231.00</td>
    </tr>
    <tr>
      <th>max</th>
      <td>2016.00</td>
      <td>4.00</td>
      <td>9975000.00</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Regroupements">Regroupements<a class="anchor-link" href="#Regroupements">&#182;</a></h2><hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La meilleure façon d'interroger des données est d'y effectuer différents regroupements.<br>
Dans notre fichier sur les médecins, par exemple, on a une colonne appelée <code>genre</code> qui nous dit si un médecin est un homme ou une femme. Cette information est représentée par deux valeurs&nbsp;: "M" ou "F".</p>
<p>La fonction <code>value_counts()</code> nous permet de compter combien il y a d'occurences de chacune de ces valeurs, donc de compter le nombre d'hommes et de femmes dans notre tableau.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[27]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[27]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>M    22441
F    12668
Name: genre, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Si on veut, plutôt, calculer le pourcentage de chacune de ces valeurs, on peut se rappeler que pandas est du bon vieux python et utiliser la fonction <code>len()</code> dans la formule suivante&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[28]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span> <span class="o">/</span> <span class="nb">len</span><span class="p">(</span><span class="n">md</span><span class="o">.</span><span class="n">genre</span><span class="p">)</span><span class="o">*</span><span class="mi">100</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[28]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>M   63.92
F   36.08
Name: genre, dtype: float64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>63,92% des médecins inscrits au tableau du Collège des médecins, donc, sont des hommes; 36,08% des femmes.</p>
<hr>
<p>On peut faire la même chose avec toutes les variables et, en combinant les fonctions <code>.value_counts()</code> et <code>.head()</code>, choisir de n'afficher qu'un nombre restreint de valeurs quand on en a plusieurs. Dans notre fichier de contrats militaires, par exemple, la formule ci-dessous nous permet d'identifier quel sont les 10 fournisseurs qui ont obtenu le plus grand nombre de contrats du ministère de la Défense.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[29]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">fournisseur</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[29]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>SIMEX DEFENCE INC. / DEFENSE SIMEX INC.                         1910
IMPERIAL OIL                                                    1608
Unisource Technology Inc                                        1315
FORD MOTOR COMPANY OF CANADA, LIMITED/FORD DU CANADA LIMITEE     957
Calian Ltd                                                       950
General Motors of Canada Limited                                 772
J.H.T. ELECTRONICS LTD.                                          714
BLUEWAVE ENERGY                                                  634
WORLD FUEL SERVICES                                              628
Imperial Oil Limited                                             601
Name: fournisseur, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Vous remarquerez cependant, ici, que le 2e et le 10e fournisseur sont la même entreprise, mais écrite d'une manière différente («IMPERIAL OIL» dans un cas, «Imperial Oil Limited» dans l'autre).<br>
Ici, donc, avant d'utiliser pandas, il serait préférable d'effectuer d'abord un nettoyage de nos données avec <a href="http://openrefine.org/">OpenRefine</a>.
<img src="https://avatars0.githubusercontent.com/u/2538880?v=3&amp;s=200" alt=""></p>
<hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Nettoyage-simple-avec-.str.replace()">Nettoyage simple avec <code>.str.replace()</code><a class="anchor-link" href="#Nettoyage-simple-avec-.str.replace()">&#182;</a></h4>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Si vos données ne requièrent pas de nettoyage trop complexe, vous pouvez utiliser la fonction <code>.str.replace()</code>.</p>
<p>C'est l'une des nombreuses fonctions permettant de traiter du texte (chaînes de caractères ou <em>strings</em>, d'où le «.str») dans pandas.</p>
<p>Dans la variable <code>md</code>, par exemple, la première colonne contient le numéro de permis de tous les médecins. Ce numéro est précédé d'un dièse ou <em>hashtag</em> (#). Vous voulez anéantir ce caractère superfétatoire. Voici comment faire.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[30]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">num</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">num</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;#&quot;</span><span class="p">,</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
<span class="n">md</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[30]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>35109 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="ATTENTION">ATTENTION<a class="anchor-link" href="#ATTENTION">&#182;</a></h4>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Les fonctions <code>.str</code> n'agissent que sur des <em>series</em>.</p>
<p>Ainsi, si vous écrivez la ligne de code suivante&nbsp;:</p>
<p><code>md = md.num.str.replace("#","")</code></p>
<p>Votre <em>dataframe</em> <code>md</code> va être remplacé <strong>au complet</strong> par une simple <em>serie</em> ne contenant que les numéros de permis des médecins.</p>
<p>On peut éviter ce fâcheux contretemps en demandant à <code>str.replace()</code> de ne transformer que la colonne <code>md.num</code>, comme je l'ai fait quelques cellules plus haut.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Dans pandas, il existe une autre fonction qui permet d'effectuer des regroupements.<br>
Il s'agit de la fonction <strong><code>.groupby()</code></strong></p>
<p>On peut alors se demander quelle est la différence entre&nbsp;:</p>
<ul>
<li><code>mil.fournisseur.value_counts()</code> et</li>
<li><code>mil.groupby("fournisseur")</code></li>
</ul>
<p>La différence est simple. Il faut se souvenir que pandas travaille avec deux grandes structures de données, les <em>series</em> et les <em>dataframes</em>.</p>
<p>Quand on fait <code>mil.fournisseur</code>, on crée une <em>series</em> à partir de <code>mil</code>. C'est tout simplement une liste de valeurs. Et la fonction <code>.value_counts()</code> ne fait que dénombrer ces valeurs. Il faut aussi savoir que cette fonction ne s'applique qu'à des <em>series</em>.</p>
<p>Quand on fait <code>mil.groupby("fournisseurs")</code> on crée en fait autant de <em>dataframes</em> qu'il y a de fournisseurs. La fonction <code>.value_counts()</code> ne fonctionne plus. Mais on peut tout de même effectuer des calculs ou des regroupements en fonction des autres colonnes qui se trouvent toujours dans nos <em>dataframe</em>, une structure de données plus complexe qu'une <em>series</em>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>C'est ainsi que s'il est intéressant de connaître le nombre de contrats que chaque fournisseur a obtenu, il est encore plus pertinent de savoir qui sont les fournisseurs qui ont décroché les contrats les plus lucratifs.</p>
<p>La fonction <code>.groupby()</code>, combinée à d'autres fonctions qu'on a vues antérieurement, va nous permettre de trouver la réponse.</p>
<p>La formule ci-dessous enchaîne cinq opérations&nbsp;:</p>
<ul>
<li>Un <em>groupby</em> avec <code>mil</code> en fonction de la colonne <code>fournisseur</code></li>
<li>On transforme chacun des <em>dataframes</em> ainsi créés en un <em>serie</em> extrait de la colonne <code>montant</code></li>
<li>On fait, avec la fonction <code>.sum()</code>, la somme des montants de chacune de ces <em>series</em></li>
<li>On les ordonne en ordre décroissant avec la fonction <code>.sort_values()</code> et le paramètre <code>ascending=**False**</code></li>
<li>On affiche les 10 premiers.</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[31]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s2">&quot;fournisseur&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[31]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>fournisseur
General Dynamics Ordnance and Tactical Systems - Canada Inc   720145247.00
UNITED STATES DEPARTMENT OF THE NAVY (NAVAIR)                 275029944.00
SIMEX DEFENCE INC. / DEFENSE SIMEX INC.                       225237149.00
UNITED STATES DEPARTMENT OF THE ARMY (USASAC)                 203107502.00
Lockheed Martin Canada Inc.                                   190692963.53
UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAC)             154954999.00
Calian Ltd.                                                   152633588.67
Valcom Consulting Group Inc.                                  151766430.97
RHEINMETALL CANADA INC.                                       140351196.40
NATO SEASPARROW SURFACE       MISSILE SYSTEM PROJECT          125042079.00
Name: montant, dtype: float64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Regroupements-conditionnels">Regroupements conditionnels<a class="anchor-link" href="#Regroupements-conditionnels">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On a vu, plus haut, comment sélectionner une partie d'un tableau en fonction des numéros de lignes ou de colonnes.<br>
Il est aussi possible de faire des sélections en fonction d'une valeur donnée. Par exemple, si, dans nos médecins, on souhait ne choisir que le groupe des médecins qui ont été radiés de leur ordre professionnel. On pourrait commencer par examiner la colonne <code>statut</code> pour voir quelles sont les différentes valeurs qu'elle contient.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[32]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">statut</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[32]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Inscrit - Actif                                            21017
Démission                                                   4623
Retrait pour décès                                          3877
Inscrit - Retraité                                          2415
Radié pour non paiement de cotisation                       2085
Expiration                                                   630
Inscrit - Actif (l&#39;exercice de ce membre est limité)         184
Radié pour non-paiement de cotisation                         88
Inscrit - Retraité (l&#39;exercice de ce membre est limité)       71
Radié                                                         67
Retrait                                                       29
Inscrit - Inactif                                             10
Non inscrit                                                    9
Révocation                                                     4
Name: statut, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On remarque qu'il y a 67 médecins dont le statut est «<strong>Radié</strong>» et 88 dont le statut est «<strong>Radié pour non-paiement de cotisation</strong>». On ne s'intéresse qu'aux premiers.</p>
<p>On va donc créer une variable que je vais appeler <code>rad</code> et je vais y mettre uniquement les médecins dont le statut est «Radié» avec la formule suivante&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[33]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">rad</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">statut</span> <span class="o">==</span> <span class="s2">&quot;Radié&quot;</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Je peux maintenant utiliser le sous-ensemble <code>rad</code> de mon tableau <code>md</code> pour effectuer toutes les opérations qu'on a vues jusqu'à maintenant.<br>
Il faut seulement se souvenir que ce sous-ensemble est désigné ainsi&nbsp;: <strong><code>md[rad]</code></strong></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[34]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">rad</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[34]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1375</th>
      <td>48004</td>
      <td>1948</td>
      <td>Alphonse</td>
      <td>Bardari</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1994-10-19</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1661</th>
      <td>49130</td>
      <td>1949</td>
      <td>Jacques</td>
      <td>Pettigrew</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1993-06-17</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2512</th>
      <td>53150</td>
      <td>1953</td>
      <td>J.-C.</td>
      <td>Paquette</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1989-08-16</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2761</th>
      <td>54174</td>
      <td>1954</td>
      <td>Philippe</td>
      <td>Moreault</td>
      <td>M</td>
      <td>Psychiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1996-04-08</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3057</th>
      <td>55201</td>
      <td>1955</td>
      <td>Claude</td>
      <td>Saint-Laurent</td>
      <td>M</td>
      <td>Psychiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>1998-07-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>21622</th>
      <td>93100</td>
      <td>1993</td>
      <td>Serge</td>
      <td>Grégoire</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-05-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>22819</th>
      <td>95451</td>
      <td>1995</td>
      <td>Jocelyn</td>
      <td>Lussier</td>
      <td>M</td>
      <td>Pédiatrie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2009-12-21</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>23026</th>
      <td>96203</td>
      <td>1996</td>
      <td>Éric</td>
      <td>Bergeron</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-04-28</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24024</th>
      <td>98262</td>
      <td>1998</td>
      <td>Yves</td>
      <td>Tremblay</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2016-04-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>27378</th>
      <td>05358</td>
      <td>2005</td>
      <td>Walif</td>
      <td>Chbeir</td>
      <td>M</td>
      <td>Radiologie diagnostique</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié</td>
      <td>2015-04-10</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>67 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Je peux donc examiner quelles sont, par exemples, les spécialités les plus courantes dans le sous-ensemble des médecins radiés.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[35]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">rad</span><span class="p">]</span><span class="o">.</span><span class="n">specialite1</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[35]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Inconnue                      29
Médecine de famille           10
Psychiatrie                    8
Chirurgie générale             6
Chirurgie plastique            3
Obstétrique et gynécologie     3
Cardiologie                    2
Médecine interne               2
Urologie                       1
Radiologie diagnostique        1
Pédiatrie                      1
Ophtalmologie                  1
Name: specialite1, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut également construire des sous-ensembles de façon plus souple en se basant sur la présence d'une chaîne de caractères donnés.<br>
Par exemple, dans nos contrats militaires, vous avez peut-être remarqué qu'il y en a plusieurs qui ont été octroyés à différentes composantes des forces armées américaines. Il y a entre autres&nbsp;:</p>
<ul>
<li>UNITED STATES DEPARTMENT OF THE ARMY</li>
<li>UNITED STATES DEPARTMENT OF THE NAVY</li>
<li>UNITED STATES DEPARTMENT OF THE AIR FORCE</li>
</ul>
<p>Si on souhaite créer un sous-ensemble regroupant tous les contrats dont le nom du fournisseur contient les mots «UNITED STATES», on peut utiliser la fonction <code>str.contains()</code> de la façon suivante&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[36]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">us</span> <span class="o">=</span> <span class="n">mil</span><span class="o">.</span><span class="n">fournisseur</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;UNITED STATES&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut ensuite faire un décompte des différents noms de fournisseurs qu'on a ainsi regroupés pour constater qu'il y a plusieurs agences américaines à qui la défense canadienne a octroyé des contrats.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[37]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="p">[</span><span class="n">us</span><span class="p">]</span><span class="o">.</span><span class="n">fournisseur</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[37]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>UNITED STATES DEPARTMENT OF THE ARMY (USASAC)         152
UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAC)     131
UNITED STATES DEPARTMENT OF THE NAVY (NAVAIR)         120
UNITED STATES DEPARTMENT OF THE NAVY (NAVSEA)          72
UNITED STATES DEPARTMENT OF THE AIR FORCE (AFSAT)      68
UNITED STATES DEPARTMENT OF THE ARMY (TRADOC)          60
UNITED STATES DEPARTMENT OF THE NAVY (NETSAFA)         55
UNITED STATES DEPARTMENT OF THE NAVY (NAVICP)          39
UNITED STATES DEPARTMENT OF THE NAVY (MISC)            35
UNITED STATES DEPARTMENT OF THE NAVY (SPAWAR)          26
UNITED STATES DEPARTMENT OF THE AIR FORCE (SAF/IA)      4
Name: fournisseur, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Et quelle est la valeur totale des contrats que ces agences ont obtenu entre 2004 et 2016?</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[38]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="p">[</span><span class="n">us</span><span class="p">]</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[38]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>1069596099.0</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Cette somme représente quelle proportion du total qui a été octroyé en contrats par le ministère de la Défense au cours de la même période?</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[39]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="p">[</span><span class="n">us</span><span class="p">]</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span> <span class="o">/</span> <span class="n">mil</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span> <span class="o">*</span> <span class="mi">100</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[39]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>3.9376522907478764</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Attention!">Attention!<a class="anchor-link" href="#Attention!">&#182;</a></h4><p>La fonction <code>str.contains()</code> est sensible à la casse. Ainsi, si on revient à nos médecins, la formule</p>
<ul>
<li><code>md.statut.str.contains("Actif")</code></li>
</ul>
<p>Ne donnera pas les mêmes résultats que</p>
<ul>
<li><code>md.statut.str.contains("actif")</code></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[40]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">actifs</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">statut</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;actif&quot;</span><span class="p">)</span>
<span class="nb">len</span><span class="p">(</span><span class="n">md</span><span class="p">[</span><span class="n">actifs</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[40]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>10</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[41]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">actifs</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">statut</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;Actif&quot;</span><span class="p">)</span>
<span class="nb">len</span><span class="p">(</span><span class="n">md</span><span class="p">[</span><span class="n">actifs</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[41]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>21201</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>La première ne regroupe que 10 médecins, tandis que la seconde en compte 21&nbsp;201!<br>
Pourquoi?</p>
<p>Parce que la première ne regroupe que les médecins dont le statut contient la chaîne «actif» avec un «a» minuscule, à savoir&nbsp;:</p>
<ul>
<li>Inscrit - Inactif</li>
</ul>
<p>La seconde comprend les médecins dont les statuts contiennent la même chaîne, mais avec un «A» majuscule, c'est-à-dire&nbsp;:</p>
<ul>
<li>Inscrit - Actif</li>
<li>Inscrit - Actif (l'exercice de ce membre est limité)</li>
</ul>
<hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>À partir de notre sous-ensemble de médecins actifs, on peut aussi créer d'autres sous-ensembles. La formule ci-dessous sélectionne les médecins de famille dans ce groupe.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[42]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">famille</span> <span class="o">=</span> <span class="n">md</span><span class="p">[</span><span class="n">actifs</span><span class="p">]</span><span class="o">.</span><span class="n">specialite1</span> <span class="o">==</span> <span class="s2">&quot;Médecine de famille&quot;</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Mais attention, si vous voulez afficher le sous-ensemble que vous venez de créer, vous pourriez être tenté d'écrire ceci&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[43]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_stream output_stderr output_text">
<pre>//anaconda3/lib/python3.7/site-packages/ipykernel_launcher.py:1: UserWarning: Boolean Series key will be reindexed to match DataFrame index.
  &#34;&#34;&#34;Entry point for launching an IPython kernel.
</pre>
</div>
</div>

<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_text output_error">
<pre>
<span class="ansi-red-fg">---------------------------------------------------------------------------</span>
<span class="ansi-red-fg">IndexingError</span>                             Traceback (most recent call last)
<span class="ansi-green-fg">&lt;ipython-input-43-3f2f0abd82e6&gt;</span> in <span class="ansi-cyan-fg">&lt;module&gt;</span>
<span class="ansi-green-fg">----&gt; 1</span><span class="ansi-red-fg"> </span>md<span class="ansi-blue-fg">[</span>famille<span class="ansi-blue-fg">]</span>

<span class="ansi-green-fg">//anaconda3/lib/python3.7/site-packages/pandas/core/frame.py</span> in <span class="ansi-cyan-fg">__getitem__</span><span class="ansi-blue-fg">(self, key)</span>
<span class="ansi-green-intense-fg ansi-bold">   2789</span>         <span class="ansi-red-fg"># Do we have a (boolean) 1d indexer?</span>
<span class="ansi-green-intense-fg ansi-bold">   2790</span>         <span class="ansi-green-fg">if</span> com<span class="ansi-blue-fg">.</span>is_bool_indexer<span class="ansi-blue-fg">(</span>key<span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">:</span>
<span class="ansi-green-fg">-&gt; 2791</span><span class="ansi-red-fg">             </span><span class="ansi-green-fg">return</span> self<span class="ansi-blue-fg">.</span>_getitem_bool_array<span class="ansi-blue-fg">(</span>key<span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">   2792</span> 
<span class="ansi-green-intense-fg ansi-bold">   2793</span>         <span class="ansi-red-fg"># We are left with two options: a single key, and a collection of keys,</span>

<span class="ansi-green-fg">//anaconda3/lib/python3.7/site-packages/pandas/core/frame.py</span> in <span class="ansi-cyan-fg">_getitem_bool_array</span><span class="ansi-blue-fg">(self, key)</span>
<span class="ansi-green-intense-fg ansi-bold">   2841</span>         <span class="ansi-red-fg"># check_bool_indexer will throw exception if Series key cannot</span>
<span class="ansi-green-intense-fg ansi-bold">   2842</span>         <span class="ansi-red-fg"># be reindexed to match DataFrame rows</span>
<span class="ansi-green-fg">-&gt; 2843</span><span class="ansi-red-fg">         </span>key <span class="ansi-blue-fg">=</span> check_bool_indexer<span class="ansi-blue-fg">(</span>self<span class="ansi-blue-fg">.</span>index<span class="ansi-blue-fg">,</span> key<span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">   2844</span>         indexer <span class="ansi-blue-fg">=</span> key<span class="ansi-blue-fg">.</span>nonzero<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">[</span><span class="ansi-cyan-fg">0</span><span class="ansi-blue-fg">]</span>
<span class="ansi-green-intense-fg ansi-bold">   2845</span>         <span class="ansi-green-fg">return</span> self<span class="ansi-blue-fg">.</span>_take_with_is_copy<span class="ansi-blue-fg">(</span>indexer<span class="ansi-blue-fg">,</span> axis<span class="ansi-blue-fg">=</span><span class="ansi-cyan-fg">0</span><span class="ansi-blue-fg">)</span>

<span class="ansi-green-fg">//anaconda3/lib/python3.7/site-packages/pandas/core/indexing.py</span> in <span class="ansi-cyan-fg">check_bool_indexer</span><span class="ansi-blue-fg">(index, key)</span>
<span class="ansi-green-intense-fg ansi-bold">   2314</span>         <span class="ansi-green-fg">if</span> mask<span class="ansi-blue-fg">.</span>any<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">:</span>
<span class="ansi-green-intense-fg ansi-bold">   2315</span>             raise IndexingError(
<span class="ansi-green-fg">-&gt; 2316</span><span class="ansi-red-fg">                 </span><span class="ansi-blue-fg">&#34;Unalignable boolean Series provided as &#34;</span>
<span class="ansi-green-intense-fg ansi-bold">   2317</span>                 <span class="ansi-blue-fg">&#34;indexer (index of the boolean Series and of &#34;</span>
<span class="ansi-green-intense-fg ansi-bold">   2318</span>                 <span class="ansi-blue-fg">&#34;the indexed object do not match).&#34;</span>

<span class="ansi-red-fg">IndexingError</span>: Unalignable boolean Series provided as indexer (index of the boolean Series and of the indexed object do not match).</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Vous obtiendrez un message d'erreur tout aussi mystérieux qu'il peut être contrariant.</p>
<p>Il faut se souvenir que «famille» a été créé à partir de «actifs», il n'existe qu'en fonction du sous-ensemble <code>md[actifs]</code>, et il faudra simplement enchaîner les deux sous-ensembles ainsi&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[44]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">actifs</span><span class="p">][</span><span class="n">famille</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[44]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4181</th>
      <td>59140</td>
      <td>1959</td>
      <td>Henri</td>
      <td>Lecoq</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4284</th>
      <td>59258</td>
      <td>1959</td>
      <td>Erwin B.</td>
      <td>Nichols</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4384</th>
      <td>60023</td>
      <td>1960</td>
      <td>Gilles</td>
      <td>Aubin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4476</th>
      <td>60118</td>
      <td>1960</td>
      <td>Paul-Émile</td>
      <td>Godin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4481</th>
      <td>60123</td>
      <td>1960</td>
      <td>Paulin</td>
      <td>Hébert</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10107 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Une autre façon d'arriver exactement au même résultat est d'effectuer de façon indépendante vos deux regroupements.<br>
On pourra créer un sous-ensemble des médecins de famille à partir de l'ensemble des médecins&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[45]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">famille</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">specialite1</span> <span class="o">==</span> <span class="s2">&quot;Médecine de famille&quot;</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Et là, écrire <code>md[famille]</code> va fonctionner (ce sous-ensemble regroupe 13&nbsp;150 médecins).</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[46]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[46]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>5</th>
      <td>30008</td>
      <td>1930</td>
      <td>Antoni</td>
      <td>Blais</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-06-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>6</th>
      <td>30012</td>
      <td>1930</td>
      <td>Lyla</td>
      <td>Brown</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1994-06-07</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>9</th>
      <td>30017</td>
      <td>1930</td>
      <td>Rémi</td>
      <td>Desjardins</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-09-23</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>13150 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Puis, pour faire une intersection avec nos 21&nbsp;201 médecins actifs, il vous suffira d'écrire ceci&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[47]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">actifs</span> <span class="o">&amp;</span> <span class="n">famille</span><span class="p">]</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[47]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4181</th>
      <td>59140</td>
      <td>1959</td>
      <td>Henri</td>
      <td>Lecoq</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4284</th>
      <td>59258</td>
      <td>1959</td>
      <td>Erwin B.</td>
      <td>Nichols</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4384</th>
      <td>60023</td>
      <td>1960</td>
      <td>Gilles</td>
      <td>Aubin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4476</th>
      <td>60118</td>
      <td>1960</td>
      <td>Paul-Émile</td>
      <td>Godin</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4481</th>
      <td>60123</td>
      <td>1960</td>
      <td>Paulin</td>
      <td>Hébert</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif (l'exercice de ce membre est l...</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35103</th>
      <td>16892</td>
      <td>2016</td>
      <td>Steve</td>
      <td>Lauwaët</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10107 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Et voilà!<br>
On sait que, dans l'ensemble des 35&nbsp;109 membres et ex-membres du Collège des médecins, on a 10&nbsp;107 médecins actifs qui sont des médecins de famille.</p>
<p>Maintenant, dans ce sous-groupe, quelle est la répartition homme/femme?</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[48]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span> <span class="o">&amp;</span> <span class="n">actifs</span><span class="p">]</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[48]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>F    5610
M    4497
Name: genre, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ce qui représente quelles proportions?</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[49]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span> <span class="o">&amp;</span> <span class="n">actifs</span><span class="p">]</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span> <span class="o">/</span> <span class="nb">len</span><span class="p">(</span><span class="n">md</span><span class="p">[</span><span class="n">famille</span> <span class="o">&amp;</span> <span class="n">actifs</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[49]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>F   55.51
M   44.49
Name: genre, dtype: float64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On a peut-être une nouvelle, ici. Chez les médecins de famille actifs, au Québec, il y a une majorité de femmes (55,5%, contre 44,5% chez les hommes).</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>On peut même faire des sous-ensembles encore plus pointus. Par exemple, quelle est la répartition homme/femme des membres du Collège des médecins qui sont chirurgiens, actifs, ayant obtenu leur diplôme depuis 2000 et pratiquant au Québec?</p>
<p>On a déjà notre sous-ensemble des médecins actifs. On va en créer trois autres.</p>
<p>D'abord les médecins pratiquant au Québec.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[50]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">qc</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">prov</span> <span class="o">==</span> <span class="s2">&quot;Québec&quot;</span>
<span class="n">md</span><span class="p">[</span><span class="n">qc</span><span class="p">]</span>
<span class="c1"># Sous-ensemble de 29 794 médecins</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[50]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>30001</td>
      <td>1930</td>
      <td>Lucien</td>
      <td>Amyot</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1981-12-29</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>1</th>
      <td>30002</td>
      <td>1930</td>
      <td>Wilfrid</td>
      <td>Audet</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1987-10-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>2</th>
      <td>30003</td>
      <td>1930</td>
      <td>A. T.</td>
      <td>Batshaw</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1983-11-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>3</th>
      <td>30005</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Beaudry</td>
      <td>M</td>
      <td>Dermatologie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-02-12</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>4</th>
      <td>30006</td>
      <td>1930</td>
      <td>P. E.</td>
      <td>Belleau</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1986-05-31</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>29794 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ensuite, les médecins ayant intégré la profession depuis 2000.<br>
Au lieu d'utiliser <code>==</code>, on va se servir d'un autre opérateur qui peut s'appliquer à des nombres.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[51]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">depuis2000</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">annee</span> <span class="o">&gt;=</span> <span class="mi">2000</span>
<span class="n">md</span><span class="p">[</span><span class="n">depuis2000</span><span class="p">]</span>
<span class="c1"># Ce sous-ensemble compte 10411 médecins</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[51]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>24698</th>
      <td>00001</td>
      <td>2000</td>
      <td>Themistocles</td>
      <td>Assimes</td>
      <td>M</td>
      <td>Médecine interne</td>
      <td>Cardiologie</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>2001-07-01</td>
      <td>Régulier</td>
      <td>Californie</td>
      <td>États-Unis</td>
    </tr>
    <tr>
      <th>24699</th>
      <td>00002</td>
      <td>2000</td>
      <td>Brian</td>
      <td>Cameron</td>
      <td>M</td>
      <td>Inconnue</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Expiration</td>
      <td>2001-01-11</td>
      <td>Temporaire</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24700</th>
      <td>00003</td>
      <td>2000</td>
      <td>François</td>
      <td>Gaumont</td>
      <td>M</td>
      <td>Médecine d'urgence</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24701</th>
      <td>00004</td>
      <td>2000</td>
      <td>Nathalie</td>
      <td>Hache</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>24702</th>
      <td>00005</td>
      <td>2000</td>
      <td>Geneviève</td>
      <td>Morin</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35104</th>
      <td>16893</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>David</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35105</th>
      <td>16894</td>
      <td>2016</td>
      <td>Guillaume Patrick Jean</td>
      <td>Berthier</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Restrictif</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35106</th>
      <td>16895</td>
      <td>2016</td>
      <td>Miriam</td>
      <td>Banoub</td>
      <td>F</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35107</th>
      <td>16896</td>
      <td>2016</td>
      <td>Anne-Sophie</td>
      <td>Lemay</td>
      <td>F</td>
      <td>Hématologie</td>
      <td>Oncologie médicale</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35108</th>
      <td>16897</td>
      <td>2016</td>
      <td>Mohamed Ali</td>
      <td>Abla</td>
      <td>M</td>
      <td>Médecine de famille</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>10411 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ensuite, on va identifier les chirurgiens.<br>
Ici, on va se servir de la fonction <code>.str.contains()</code> pour réunir tous les MD dont la spécialité contient l'expression «hirurgie», ce qui permet de repérer autant «C<strong>hirurgie</strong> générale» que «Neuroc<strong>hirurgie</strong>».</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[52]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">chir1</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">specialite1</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;hirurgie&quot;</span><span class="p">)</span>
<span class="n">md</span><span class="p">[</span><span class="n">chir1</span><span class="p">]</span>
<span class="c1"># On en obtient 3 259</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[52]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>7</th>
      <td>30014</td>
      <td>1930</td>
      <td>Alphonse</td>
      <td>Couturier</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1995-08-11</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>8</th>
      <td>30015</td>
      <td>1930</td>
      <td>Guy</td>
      <td>D'Argencourt</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Radié pour non-paiement de cotisation</td>
      <td>1988-11-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>30</th>
      <td>30063</td>
      <td>1930</td>
      <td>Arthur M.</td>
      <td>Vineberg</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1988-03-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33</th>
      <td>30072</td>
      <td>1930</td>
      <td>Maurice</td>
      <td>Berne</td>
      <td>M</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1993-06-24</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>38</th>
      <td>30080</td>
      <td>1930</td>
      <td>C. Emerson</td>
      <td>Brooks</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Démission</td>
      <td>1977-06-30</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>35028</th>
      <td>16795</td>
      <td>2016</td>
      <td>Mohamed Akli</td>
      <td>Zetchi</td>
      <td>M</td>
      <td>Neurochirurgie</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Ontario</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35031</th>
      <td>16799</td>
      <td>2016</td>
      <td>Sara</td>
      <td>Langlais</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35034</th>
      <td>16802</td>
      <td>2016</td>
      <td>Gabrielle</td>
      <td>Roy</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35060</th>
      <td>16838</td>
      <td>2016</td>
      <td>Hussein</td>
      <td>Wissanji</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>35061</th>
      <td>16839</td>
      <td>2016</td>
      <td>Sébastien</td>
      <td>Lachance</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>3259 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il faut également vérifier les médecins dont la 2e ou 3e spécialité est la chirurgie, car on a trois colonnes de spécialités.<br>
Il faudra cependant ajouter un paramètre à la fonction <code>.str.contains</code> qui va faire en sorte d'ignorer les médecins qui n'ont aucune 2e ou 3e spécialité avec l'argument <code>na=False</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[53]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">chir2</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">specialite2</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;hirurgie&quot;</span><span class="p">,</span> <span class="n">na</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">md</span><span class="p">[</span><span class="n">chir2</span><span class="p">]</span>
<span class="c1"># On obtient ici 268 médecins</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[53]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>19</th>
      <td>30042</td>
      <td>1930</td>
      <td>Marcel</td>
      <td>Ostiguy</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1994-10-15</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>30</th>
      <td>30063</td>
      <td>1930</td>
      <td>Arthur M.</td>
      <td>Vineberg</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1988-03-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>69</th>
      <td>31050</td>
      <td>1931</td>
      <td>Gérard</td>
      <td>Rolland</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1989-10-28</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>74</th>
      <td>31059</td>
      <td>1931</td>
      <td>L. J.</td>
      <td>Tessier</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>2002-12-26</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>99</th>
      <td>32011</td>
      <td>1932</td>
      <td>J. A.</td>
      <td>Bohemier</td>
      <td>M</td>
      <td>Ophtalmologie</td>
      <td>Oto-rhino-laryngologie / chirurgie cervico-fac...</td>
      <td>NaN</td>
      <td>Retrait pour décès</td>
      <td>1996-04-01</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>31776</th>
      <td>12698</td>
      <td>2012</td>
      <td>Heather</td>
      <td>Gill</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>32003</th>
      <td>13111</td>
      <td>2013</td>
      <td>Dominique</td>
      <td>Boudreau</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie générale oncologique</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33100</th>
      <td>14430</td>
      <td>2014</td>
      <td>Mireille</td>
      <td>Méthot</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>33151</th>
      <td>14481</td>
      <td>2014</td>
      <td>Ricardo</td>
      <td>Ruz</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie vasculaire</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>34481</th>
      <td>16207</td>
      <td>2016</td>
      <td>Mai-Kim</td>
      <td>Gervais</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie générale oncologique</td>
      <td>NaN</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
<p>268 rows × 13 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[54]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">chir3</span> <span class="o">=</span> <span class="n">md</span><span class="o">.</span><span class="n">specialite3</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">contains</span><span class="p">(</span><span class="s2">&quot;hirurgie&quot;</span><span class="p">,</span> <span class="n">na</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">md</span><span class="p">[</span><span class="n">chir3</span><span class="p">]</span>
<span class="c1"># Quatre médecins dans ce sous-ensemble</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[54]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num</th>
      <th>annee</th>
      <th>prenom</th>
      <th>nom</th>
      <th>genre</th>
      <th>specialite1</th>
      <th>specialite2</th>
      <th>specialite3</th>
      <th>statut</th>
      <th>date</th>
      <th>typePermis</th>
      <th>prov</th>
      <th>pays</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>313</th>
      <td>36013</td>
      <td>1936</td>
      <td>J. Ernest</td>
      <td>Bousquet</td>
      <td>M</td>
      <td>Chirurgie thoracique</td>
      <td>Pneumologie</td>
      <td>Chirurgie générale</td>
      <td>Retrait pour décès</td>
      <td>1983-11-06</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>10671</th>
      <td>74293</td>
      <td>1974</td>
      <td>Pierre</td>
      <td>Michaud</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie thoracique</td>
      <td>Chirurgie vasculaire</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>12161</th>
      <td>76365</td>
      <td>1976</td>
      <td>Louise</td>
      <td>Choiniere</td>
      <td>F</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie cardio-vasculaire et thoracique</td>
      <td>Chirurgie thoracique</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
    <tr>
      <th>16006</th>
      <td>82154</td>
      <td>1982</td>
      <td>Rosaire</td>
      <td>Vaillancourt</td>
      <td>M</td>
      <td>Chirurgie générale</td>
      <td>Chirurgie cardio-vasculaire et thoracique</td>
      <td>Chirurgie thoracique</td>
      <td>Inscrit - Actif</td>
      <td>NaN</td>
      <td>Régulier</td>
      <td>Québec</td>
      <td>Canada</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Si on veut les réunir tous et y voir la répartition homme/femme, la formule ci-dessous les combine de la façon suivante&nbsp;:</p>
<p>Médecins actifs <strong>ET</strong><br>
pratiquant au Québec <strong>ET</strong><br>
depuis 2000 <strong>ET</strong><br>
dont la spécialité&nbsp;1 <strong>OU</strong> la spécialité&nbsp;2 <strong>OU</strong> la spécialité&nbsp;3 est une forme ou une autre de chirurgie.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[55]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">actifs</span> <span class="o">&amp;</span> <span class="n">qc</span> <span class="o">&amp;</span> <span class="n">depuis2000</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">chir1</span> <span class="o">|</span> <span class="n">chir2</span> <span class="o">|</span> <span class="n">chir3</span><span class="p">)]</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[55]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>M    482
F    280
Name: genre, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Au tout début de notre carnet, on a importé cette bibliothèque au nom affeux, <strong>matplotlib</strong>.<br>
On va s'en servir pour créer des graphiques. Pour ce faire, il suffit d'ajouter la fonction <code>.plot()</code> à la fin d'une formule.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[56]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span> <span class="o">&amp;</span> <span class="n">actifs</span><span class="p">]</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[56]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x118e64278&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Ce n'est pas très évocateur. On peut heureusement changer le type de graphique pour, par exemple, choisir un graphique en pointes de tarte. Il suffit d'ajouter, à la fonction <code>.plot()</code> l'argument <code>kind</code> auquel on donne la valeur de <code>pie</code>.<br>
On peut aussi donner un titre à notre graphique avec l'argument <code>title</code>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[57]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="p">[</span><span class="n">famille</span> <span class="o">&amp;</span> <span class="n">actifs</span><span class="p">]</span><span class="o">.</span><span class="n">genre</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">kind</span><span class="o">=</span><span class="s2">&quot;pie&quot;</span><span class="p">,</span> <span class="n">title</span><span class="o">=</span><span class="s2">&quot;Majorité de femmes médecin de famille au Québec&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[57]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x118ea5198&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Un autre type de graphique intéressant est l'histogramme.<br>
Pour tracer l'évolution du nombre de médecins ayant intégré la profession médicale au cours des ans, on pourrait faire un histogramme de notre tableau <code>md</code> en fonction de la colonne <code>annee</code> avec la formule suivante&nbsp;:</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[58]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">annee</span><span class="o">.</span><span class="n">hist</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[58]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x1172bc4e0&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Mais voilà qui ne raconte pas grand-chose. C'est que par défaut, l'histogramme trace 10 barres, ce qui fait que chaque barre de notre histogramme regroupe 7 ou 8 années.<br>
Les barres, c'est que ce matplotlib appelle des <em>«bins»</em>. On peut ainsi spécifier le nombre de ces <em>bins</em> avec un argument qui s'appelle... vous l'aurez deviné... <code>bins</code></p>
<p>Ici, comme nos données couvrent 87 années, on va créer 87 barres.<br>
Chacune représente le nombre de médecins qui ont obtenu leur permis de pratique au cours d'une année donnée.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[59]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">annee</span><span class="o">.</span><span class="n">hist</span><span class="p">(</span><span class="n">bins</span><span class="o">=</span><span class="mi">87</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[59]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x1194ec940&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Il remarque une chute au début des années 1990. Elle correspond à une politique du gouvernement québécois qui avait limité le nombre d'inscriptions dans les facultés de médecine quelques années auparavant.</p>
<p>Inspiré par ce graphique, vous pourriez avoir envie de voir combien d'hommes et de femmes sont devenus médecin au fil des ans afin de visualiser la féminisation de la profession médicale. Pour ce faire, il suffirait de modifier la formule ci-dessus en ajoutant un <code>groupby</code> par <code>genre</code>, puis l'argument <code>alpha</code> à la fonction <code>.hist()</code> pour faire en sorte que nos barres aient une transparence de 50%.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[60]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">md</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s2">&quot;genre&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">annee</span><span class="o">.</span><span class="n">hist</span><span class="p">(</span><span class="n">bins</span><span class="o">=</span><span class="mi">87</span><span class="p">,</span><span class="n">alpha</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[60]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>genre
F    AxesSubplot(0.125,0.125;0.775x0.755)
M    AxesSubplot(0.125,0.125;0.775x0.755)
Name: annee, dtype: object</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Le graphique ci-dessus raconte une histoire avec les données.</p>
<p>On y voit que jusqu'en 1970, les hommes (en jaune) étaient clairement majoritaires dans la profession.<br>
À partir de 1970 semble s'opérer un renversement. Le nombre d'hommes diminue progressivement pour, dès 1990, devenir inférieur au nombre de femmes (en bleu).<br>
Aujourd'hui, les deux tiers des recrues, en médecine, chaque année, sont des femmes.</p>
<hr>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>En terminant, faisons aussi un graphique avec nos données de contrats.<br>
Calculons la somme des contrats octroyés chaque année, créons un diagramme à barres horizontales (<code>kind="barh"</code>) et donnons une couleur de camouflage (<em>teal</em>) à nos barres.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[61]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">mil</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s2">&quot;annee&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">montant</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">kind</span><span class="o">=</span><span class="s2">&quot;barh&quot;</span><span class="p">,</span><span class="n">color</span><span class="o">=</span><span class="s2">&quot;teal&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[61]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x1175088d0&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h4 id="Voil&#224;!-J'esp&#232;re-que,-gr&#226;ce-&#224;-pandas,-vous-aurez-un-peu-de-plaisir-&#224;-explorer-vos-donn&#233;es!">Voil&#224;! J'esp&#232;re que, gr&#226;ce &#224; pandas, vous aurez un peu de plaisir &#224; explorer vos donn&#233;es!<a class="anchor-link" href="#Voil&#224;!-J'esp&#232;re-que,-gr&#226;ce-&#224;-pandas,-vous-aurez-un-peu-de-plaisir-&#224;-explorer-vos-donn&#233;es!">&#182;</a></h4>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[&nbsp;]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span> 
</pre></div>

    </div>
</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>
