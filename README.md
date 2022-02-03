# Cook's Ingredients
Collection of all the wordlists for using in [cook](https://github.com/giteshnxtlvl/cook)

### Currently fetched
- [Assetnotes Wordlsits](https://wordlists.assetnote.io/)
- [Seclist](https://github.com/danielmiessler/SecLists)
- [FuzzDB](https://github.com/fuzzdb-project/fuzzdb)
- [Bruteforce Database](https://github.com/duyet/bruteforce-database)
- [Bruteforce Lists](https://github.com/random-robbie/bruteforce-lists)
- [OneListForAll](https://github.com/six2dez/OneListForAll)

### To Fetch
http://ftp.funet.fi/pub/unix/security/passwd/crack/dictionaries/

### Customize
<img src="https://github.com/giteshnxtlvl/cook/raw/dev2/assets/folder%20structure.png">

### Creating yaml file for any repo
1. Download that repo
2. Move to its directory
3. Replace the url of repo in the below command
4. Run the command and save the output
5. Open file and add `files:` at the top.
6. Add tab before rest of the lines.
7. Put the file in `cook-ingredient` folder and you are done.
```
git ls-tree -r master --name-only | grep .txt$ | cook -p - p.fb " : [" https://raw.githubusercontent.com/username/repo/master/ p ] -append 3 
```
> Cook 2.0 needed for above command
