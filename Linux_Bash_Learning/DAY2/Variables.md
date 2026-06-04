#!/bin/bash

myname="Sara"  -> declaring string variable 
echo $myname -> using distinction "$" to print variable 
ls="Hello World!" -> using same variable name as ls cmd
echo ls -> without extinction "$" it will print list storage not the variable
echo $ls -> one of the reason why ext "$" is used to print var
clear -> clear out the cmd 
exit  -> logout
cd .. -> one step before in the directory

echo "Hello! My name is $myname."  -> double quote - variable gets printed
echo "I'm $myage year old." -> double quote - variable gets printed
echo 'Hello! My name is $myname.' -> single quote - variable NOT printed (shows as literal text)
echo 'I'\''m $myage year old.' -> single quote with escaped quote - way to add quote in single quote 

date -> prints current date and time to screen
now=$(date) -> store date output in variable 'now' using command substitution $()
echo $now -> print the date stored in variable

env -> shows all environment variables available in system
echo $TERM -> print TERM variable (terminal type)
echo $USER -> print USER variable (current logged in user)
