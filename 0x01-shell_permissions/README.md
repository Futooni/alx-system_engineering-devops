
<h1>Description</h1>



<h4>0. My name is Betty</h4>


* Script that switches the current user to the user betty.

```
#!/bin/bash
su betty
```


<h4>1. Who am I</h4>


* Script that prints the effective username of the current user.

```
#!/bin/bash
whoami
```


<h4>2. Groups</h4>


* Sccript that prints all the groups the current user is part of.

```
#!/bin/bash
groups
```


<h4>3. New owner</h4>


* Script that changes the owner of the file hello to the user betty.

```
#!/bin/bash
sudo chown betty hello 
```


<h4>4. Empty!</h4>


* Script that creates an empty file called hello.

```
#!/bin/bash
touch hello 
```


<h4>5. Execute</h4>

* Script that creates an empty file called hello.

```
#!/bin/bash
touch hello 
```

<h4> 6. Multiple permissions </h4>



* Script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

	_The file hello will be in the working directory._

```
#!/bin/bash
chmod u+x,g+x,o+r hello
```


<h4>7. Everybody!</h4>


* Script that adds execution permission to the owner, the group owner and the other users, to the file hello

	_The file hello will be in the working directory_

	_You are not allowed to use commas for this script_


```
#!/bin/bash
chmod ugo+x hello
```


<h4>8. James Bond</h4>


* Script that sets the permission to the file hello as follows:

	_Owner: no permission at all_

	_Group: no permission at all_

	_Other users: all the permissions_

*The file hello will be in the working directory You are not allowed to use commas for this script*

```
#!/bin/bash
chmod 007 hello
```


<h4>9. John Doe</h4>


* Script that sets the mode of the file hello to this:

```
-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
```

	_The file hello will be in the working directory_

	_You are not allowed to use commas for this script_


```
#!/bin/bash
chmod 753 hello
```


<h4>10. Look in the mirror </h4>


* Script that sets the mode of the file hello the same as olleh’s mode.

	_The file hello will be in the working directory_

	_The file olleh will be in the working directory_

	Note: the mode of olleh will not always be 664. Make sure your script works for any mode.

```
#!/bin/bash
chmod --reference=olleh hello
```


<h4>11. Directories</h4>


* Script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.Regular files should not be changed.

```
#!/bin/bash
chmod -R +111 */
```


<h4>12. More directories</h4>


* Script that creates a directory called my_dir with permissions 751 in the working directory.

```
#!/bin/bash
mkdir -m 751 my_dir
```


<h4>13. Change group</h4>


* Script that changes the group owner to school for the file hello

	_The file hello will be in the working directory_

```
#!/bin/bash
chgrp school hello
```


<h4>14. Owner and group</h4>


* Script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

```
#!/bin/bash
chown vincent:staff *
```


<h4>15. Symbolic links</h4>


* Script that changes the owner and the group owner of _hello to vincent and staff respectively.

	_The file _hello is in the working directory_

	_The file _hello is a symbolic link_


```
#!/bin/bash
chown -h vincent:staff _hello
```


<h4>16. If only</h4>


* Script that changes the owner of the file hello to betty only if it is owned by the user guillaume.

	_The file hello will be in the working directory_

```
#!/bin/bash
chown --from=guillaume betty hello
```


<h4>17. Star Wars</h4>


* Script that will play the StarWars IV episode in the terminal.

```
#!/bin/bash
telnet towel.blinkenlights.nl
```

