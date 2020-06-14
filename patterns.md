Delete the first number on all lines that start with a "#,"
`sed '/^# s/[0-9][0-9]*//`

Change delimiter by ,
`sed '\,^#, s/[0-9][0-9]*//'`

Remoing commant+blank line
`sed -e 's/#.*//' -e '/^$/ d'`
