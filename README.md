README.md



## 1. Steroid-Aliases

### Un file .bash_aliases customizzato secondo le varie esigenze emerse negli anni 

Tip: Per evidenziare i comandi più usati e creare quindi degli aliases, potete usare questo oneliner: "tophist", l'alias è già presente nel file.

```shell
#creare l'alias
#Attenzione agli escapes \ usati per awk
alias tophist="history | awk '{CMD[\$2]++;count++;}END { for (a in CMD)print CMD[a] \" \" CMD[a]/count*100 \"% \" a;}' | grep -v \"./ \" | column -c3 -s \" \" -t | sort -nr | nl |  head -n10"
```
