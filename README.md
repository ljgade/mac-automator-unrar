# mac-automator-unrar
```
current_path=`dirname "$1"`
echo "$current_path"
for f in "$@"
do
	if [ -f "$f" ]
	then
		/usr/local/bin/unrar x "$f" ~/Downloads/
	fi
done
```