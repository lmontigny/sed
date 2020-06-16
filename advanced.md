- Multiple commands with `;`  
`sed 's/and/\&/;s/people/horses/' song.txt`

- Insert blank line for each line  
`sed 'G' song.text`

- Replace on the line containing 'it' for example  
`sed '/it/s/goes/now/' song.txt`

- Print every 5th line starting from 2  
`first~step`
`sed -n '2~5p' BSD.txt`

- Replace every 2nd occurence on each line  
`sed 's/on/forward/2' song.txt`

- Ignore case  
`sed 's/on/forward/i' song.txt`

- Replace from begining to 'at'  
`sed 's/on/forward/2' song.txt`






