
<h1> Description </h1>
**0x03. Shell, init files, variables and expansions project**


<h3>0. <o></h3>

**Create a script that creates an alias.**

* Name: ls
* Value: rm *

```
#!/bin/bash
alias ls="rm *"
```


<h3>1. Hello you</h3>

**Create a script that prints _hello user_, where user is the current Linux user.**

```
#!/bin/bash
echo "hello $USER"
```

<h3>2. The path to success is to take massive, determined action</h3>

**Add _/action_ to the _PATH_. _/action_ should be the last directory the shell looks into when looking for a program.**

```
#!/bin/bash
PATH=$PATH:/action
```

<h3>3. If the path be beautiful, let us not ask where it leads</h3>

**Create a script that counts the number of directories in the _PATH_.**

```
#!/bin/bash
echo $PATH | tr ':' '\n' | wc -l
```


<h3>4. Global variables</h3>

**Create a script that lists environment variables.**

```
#!/bin/bash
printenv
```

<h3>5. Local variables</h3>

**Create a script that lists all local variables and environment variables, and functions.**

```
#!/bin/bash
set
```


<h3>6. Local variable</h3>

**Create a script that creates a new local variable.**

* Name: BEST
* Value: School
```
#!/bin/bash
BEST="School"
```

<h3>7. Global variable</h3>

**Create a script that creates a new global variable.**

* Name: BEST
* Value: School
```
#!/bin/bash
export BEST="School"
```


<h3>8. Every addition to true knowledge is an addition to human power</h3>

**Write a script that prints the result of the addition of 128 with the value stored in the
environment variable _TRUEKNOWLEDGE_, followed by a new line.**
```
#!/bin/bash
echo $((128 + $TRUEKNOWLEDGE))
```


<h3>9. Divide and rule</h3>

**Write a script that prints the result of _POWER_ divided by _DIVIDE_, followed by a new line.**

* _POWER_ and _DIVIDE_ are environment variables.
```
#!/bin/bash
echo $((POWER/DIVIDE))
```


<h3>10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath</h3>

**Write a script that displays the result of _BREATH_ to the power _LOVE_.**

* _BREATH_ and _LOVE_ are environment variables
* The script should display the result, followed by a new line
```
#!/bin/bash
echo $((BREATH**LOVE))
```

<h3>11. There are 10 types of people in the world -- Those who understand binary, and those who don't</h3>

**Write a script that converts a number from base 2 to base 10.**

* The number in base 2 is stored in the environment variable _BINARY_
* The script should display the number in base 10, followed by a new line
```
#!/bin/bash
echo $((2#$BINARY))
```

<h3>12. Combination</h3>

**Create a script that prints all possible combinations of two letters, except _oo_.**

* Letters are lower cases, from _a_ to _z_
* One combination per line
* The output should be alpha ordered, starting with aa
* Do not print _oo_
* Your script file should contain maximum 64 characters
```
#!/bin/bash
echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo"
```


<h3>13. Floats</h3>

**Write a script that prints a number with two decimal places, followed by a new line.**
**The number will be stored in the environment variable _NUM_.**
```
#!/bin/bash
printf '%.2f\n' $NUM
```

