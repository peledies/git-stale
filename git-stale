#!/bin/bash    

if [[ "$1" != "" ]]
then
  FILTER="$1"
else
  FILTER="Deac"
fi

for ref in $(git for-each-ref --sort=-committerdate --format="%(refname:short)" refs/remotes);
do
  git log -n1 $ref --pretty=format:"%Cgreen%cr%Creset | %C(yellow)%d%Creset% | %C(bold cyan)%an%Creset%n" | grep $FILTER |   
      while IFS='|' read date message author
      do
        printf '%-25s %35s %30s\n' "$date" "$author" "$message"
      done
done