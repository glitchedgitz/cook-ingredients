# Cook's Wordlists Database
Collection of all the wordlists for using in [cook](https://github.com/giteshnxtlvl/cook)

### Currently fetched
- [Assetnotes Wordlsits](https://wordlists.assetnote.io/)
- [Seclist](https://github.com/danielmiessler/SecLists)
- [FuzzDB](https://github.com/fuzzdb-project/fuzzdb)

### Todo
http://ftp.funet.fi/pub/unix/security/passwd/crack/dictionaries/

### Creating yaml file for any repo
1. Download that repo
2. Move to its directory
3. Replace the url of repo in the below command
4. Run the command and save the output
5. Open file and add `files:` at the top.
6. Add tab before rest of the lines.
7. Put in the `cook` database folder and you are done.
```
git ls-tree -r master --name-only | grep .txt$ | cook -a - a.fb " : [" https://raw.githubusercontent.com/fuzzdb-project/fuzzdb/master/ a ] -append 3 
```
> Cook 2.0 needed for above command
