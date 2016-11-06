
cat menu3.sh 

menu1(){                    
cat <<END
    *****************************
    1.[install lamp]
    2.[install lnmp]
menu1(){
cat <<END
    *****************************
    1.[install lamp]
    2.[install lnmp]
    3.[exit]
    pls input the num you want:
    *****************************
END
}
menu2(){
cat <<END
    ===================================
    1.[install apache]
    2.[install php]
    3.[install mysql]
    4.[back]
    pls input the 2 menu num you want:
    ===================================
END
}
menu1         
read num
[ $num -eq 1 ] &&{    
  menu2
  read num2
  [ $num2 -eq 1 ] &&{      
  echo "start installing apache."
  exit
  }
}
