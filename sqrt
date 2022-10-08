variable sqrt1
variable sqrt2
: numb-hack
	dup 10 / 10 * dup rot swap - swap
	dup 100 / 100 * dup rot swap - swap
	dup 1000 / 1000 * dup rot swap - swap
	1000 / >r + + r> swap 
;
: sqrt
 dup 1 + 1000 * 2 / 1000000
 swap 
 sqrt2 !
 *
 sqrt1 !
 begin
 			sqrt2 @
 			dup
 			sqrt1 @
 			swap
 			/
 			+ 2 /
 			dup
 			sqrt2 @
 			swap
 			sqrt2 !
 			=
 until
 sqrt2 @ 
 numb-hack
;
