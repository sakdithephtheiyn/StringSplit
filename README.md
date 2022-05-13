# StringSplit
Func _FileGetExt($sFn) ; Parse EXTension from [d:\path\]filename.EXTension     Local $sExt = "", $aA     If StringInStr($sFn, ".") Then         If Not StringInStr(FileGetAttrib($sFn), "D") Then             $aA = StringSplit($sFn, ".")             $sExt = $aA[$aA[0]]         EndIf     EndIf     Return $sExt EndFunc  ;==>_Fi
