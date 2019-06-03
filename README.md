# fbctf_challenges
2019 fbctf challenges details in json and its files

[1] json are dump after end of the game, so the total of solves are final results. But the team/user name still might change, e.g. the champion "g+" change the name to 'Visit g.co/ctf' after dump.  
[2] The files SOMBRERO_ROJO.tar.gz and SOMBRERO_ROJO_2.tar.gz seems like the same file.  
[3] Challenge id 4 doesn't exists.  
[4] json dump from team whose gained 1 point and above, 0 point will not dump. But all user of that team will get dump even though user gained 0 point.  
[5] You can issue `cat * | jq -M` command to pretty print all json files, and also `jq .data.solves ./*` to get data's solves's value inside challenges_json/ directory, or simple loop `find . -type f -exec bash -c "python -m json.tool {} | grep 'solves' "  \;`  


