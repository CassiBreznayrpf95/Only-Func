# Only-Func
ample of use:  Local $Net_Result[3] Local $NetAdrs[5] = ["localhost", @ComputerName, "127.0.0.1", "www.google.com", "216.34.181.60"] For $i = 0 To UBound($NetAdrs) - 1     $Net_Result = _mLookup($NetAdrs[$i])     ConsoleWrite($Net_Result[0] &amp; @TAB &amp; $Net_Result[1] &amp; @CRLF) Next    ; This Function accepts either an IPaddress or a Host/Domain name and returns ; a 3 elements array element[0]=IPaddress element[1]=hostname.domain element[2]=hostnameOnly Func _mLookup($Net_ID)     Local $Net_Names[3]
