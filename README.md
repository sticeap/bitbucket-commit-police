#Bitbucket Commit Police

drag [the bitbucket commit police bookmarklet link]('javascript:!function(){function t(t){for(var e=Object.keys(f),r=0,i=e.length;i>r;r++)if(!f[e[r]](t))return console.warn("failed:",e[r],t),e[r];return!0}function e(){return".iterable-item[data-commit-police]{position:relative}.iterable-item[data-commit-police]:after{position:absolute;content:attr(data-commit-police);border-radius:5px;padding:5px 10px;background:rgba(255,0,0,.8);box-shadow:0 0 4px #222;text-shadow:0 0 1px rgba(0,0,0,0.3);border:1px solid #000;color:#000;left:200px;transform:translate(0) scale(.0001);opacity:0;transition:all .1s ease-in-out;z-index:999}.iterable-item[data-commit-police]:hover:after{transform:translate(-100%,0) scale(1);opacity:1}"}function r(){$("#commit-police-styles").length||$('<style id="commit-police-styles" type="text/css"/>').text(e()).appendTo("head")}function i(){$(u).each(function(e,r){var i=$(r),n=i.text();testsReturnValue=t(n),success=testsReturnValue===!0,color=m[success],success||i.closest(".iterable-item").attr("data-commit-police",testsReturnValue),$(r).css("color",color)})}function n(){r(),i()}function o(t){return/[A-Z]/.test(t)}function a(t){return!!t}function s(t){if(!t)return!1;var e=t[0];if("["===e){if(!/^\[.*?\]/.test(t))return!1;if(e=t.replace(/^\[.*?\]\s*(.*)/,"$1")[0],!e)return!1}return o(e)}function c(t){var e=72;return t&&t.length<=e}function l(t){return/[a-z0-9]\n?$/i.test(t)}var u="#commit-list-container .iterable-item:not(.merge) .subject",f={_messageExists:a,startsWithCapitalLettter:s,hasDesiredSubjectLength:c,doesNotEndWithDot:l},m={"true":"green","false":"red"};n()}();') to your bookmarks bar and click it while you're vieweing the commits on bitbucket!

