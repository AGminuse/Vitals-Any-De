# Vitals-Any-De

It's a dirty, light script to show the real-time usage of the device on any desktop environment that supports a script or a shell command extension.


## Installation

1. Make sure to install the python-psutil from your default Package Manager. 

2. Install the vitals-any-de and place it in $HOME/.local/bin (for only this user), or you can put it in /usr/bin (for any user). 

Done 👏
#### Method 1: For Extensions that run the Command Once 
1. Add the following command in the command field. 
``` vitals-any-de -v```
   
#### Method 2: For Extensions that continuously execute the command

2.1: Run the vitals-any-de  manually using the command 
```vitals-any-de &``` 
	or set it to run at startup

2.2: Add the following command in the command field of the extension.
``` echo -e $(cat /tmp/vitels)```
 
## Customizing
1.1 You can change the emojis using the option --set-emojis like this.

``` vitals-any-de --set-emojes 💅🫱🖖🫳S✌```


1.2 or removing them by using the option --no-emojes like this 

``` vitals-any-de --no-emojes ```

2.1 You can remove any usage you don't like using any of these options. 
```
--no-desk 
--no-cpu 
--no-memory 
--no-network 
```
Exampil: To remove the emojes and disk, CPU usage.

```vitals-any-de --no-emojes --no-desk --no-cpu ```



2.2  by defult the disk usage will output the read and write combined (read+write) and the emoje will depend on which theme is greater. 
If you want to show the read and write sequentially, you can use the option 
``` --separate-disk-usage```
