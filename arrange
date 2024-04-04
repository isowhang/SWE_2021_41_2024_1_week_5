#!/bin/bash
#mkdir -p {a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,v,w,x,y,z}

find ./files | while read -r input
do 
    name=`basename $input`
    filename="${name%.*}"
    first="${filename:0:1}"
    low_first=${first,}
    if [[ $low_first =~ ^[a-z]+$ ]];then
        dst="$low_first/"
        mv $input $dst
    fi
done