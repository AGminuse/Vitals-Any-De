
# Vitals-Any-De

Its a dirty,light,Stuped soulotion to show the real time usage of the device on any Desktop Enviroment that support script or a shell command extension


## Installation

1- make sure to install the python-psutil from your default Package Manager  

2- install the vitals-any-de file and put it in $HOME/.local/bin (for only this user)  

Done 👏




## Usage 
there is alote of wayes you can use this scrip but there is two main wayes  

#### Mode 1 :  For Extensions that runs the Command Once 
1- add he following command in the command field 
``` vitals-any-de -v```
   
#### Mode 2 :  For Extensions that runs the Command more than Once

2.1- make the file vitals-any-de run at start up or run it manually by running the command 
```vitals-any-de &``` 

2.2- add he following command in the command field of the Extension
``` echo -e  $(cat /tmp/vitels)```



## Customizing

$ you can change the emojis using the option --set-emojes like this

``` vitals-any-de --set-emojes 💅🫱🖖🫳S✌```
 
or removing them by using the option --no-emojes like this 

``` vitals-any-de --no-emojes ```


$ you can remove any usage you dont like using any of this options  

``` --no-desk 
    --no-cpu 
    --no-memory 
    --no-network 
```
Exampil

```vitals-any-de --no-emojes --no-desk --no-cpu ```

this will remove the emojes and disk, cpu usage

$ by defult the disk usage will output the read and write compined (read+write) and the emoje will deppend on which of theme  is greater 

if you want to show the read and write sepretly you can use the option 

``` --separate-disk-usage```