\ some empty stacks
1 drop
1 dup drop drop
1 2 over drop drop drop
1 2 2drop

1 2 swap swap            . . ( 1 2 )
1 2 3 rot rot rot        . . . ( 1 2 3 )
1 2 3 4 2swap 2swap      . . . . ( 1 2 3 4 )

1 2 3 over               . . . . ( 1 2 3 2 )
1 2 3 dup                . . . . ( 1 2 3 3 )

\ nip
1 2 swap drop            . ( 2 )
1 2 nip                  . ( 2 )

\ tuck
1 2 dup rot rot          . . . ( 2 1 2 )
1 2 tuck                 . . . ( 2 1 2 )

\ reverse 3
3 2 1 swap rot           . . . ( 1 2 3 )

\ reverse 4
4 3 2 1 swap 2swap swap  . . . . ( 1 2 3 4 )

: nip ( a b -- b )
   swap drop ;

: tuck ( a b -- b a b )
   dup rot rot ;

: negate ( a -- -a )
   0 swap - ;

: /mod ( a b -- [a mod b] [# times b goes into a whole] )
   2dup mod rot rot / ;
