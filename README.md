```bash
#!/bin/bash

read -p 'What is your favourite OS? ' useros

useros=$( echo $useros | tr [A-Z] [a-z] )

if [ $useros = 'linux' ] ; then
	echo 'Good choice'
elif [ $useros = 'windows' ] || [ $useros = 'macos' ] ; then
	echo 'Why are you still not using linux?'
fi

exit 0
```
