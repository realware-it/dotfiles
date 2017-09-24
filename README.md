README.md



## 1. Bash aliases

Un file .bash_aliases customizzato secondo le varie esigenze emerse negli anni 

Tip: Per evidenziare i comandi più usati e creare degli aliases utili a velocizzare i comandi, potete usare questo oneliner: "tophist"

```shell
#creare l'alias
alias tophist="history | awk '{CMD[\$2]++;count++;}END { for (a in CMD)print CMD[a] \" \" CMD[a]/count*100 \"% \" a;}' | grep -v \"./ \" | column -c3 -s \" \" -t | sort -nr | nl |  head -n10"

#Attenzione agli escapes \ usati per awk

```
