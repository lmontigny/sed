# sed basic example

Delete line 1
`sed -e '1d' /etc/services | less`

Delete line 1 to 20
`sed -e '1,20d' /etc/services | less`

Delete with regex
`sed -e '/^#/d' /etc/services | less`

Print matching pattern
`sed -n -e '/^#/p' /etc/services | less`

Substitution
`sed -e 's/nfs/ftp/g' /etc/services | less`
