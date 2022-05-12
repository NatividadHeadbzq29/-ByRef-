# -ByRef-
Func _StringGetDigitLeft(Const ByRef $sString) ;   Return String(Number($sString)) ; requires at least one leading digit     Return StringRegExpReplace($sString, "^(?|(\d+)|())(.*$)", "$1") EndFunc  Func _StringGetDigitRight(Const ByRef $sString)     Return StringRegExpReplace($sString, "(.*?)(?|(\d+)|())$", "$2") EndFunc
