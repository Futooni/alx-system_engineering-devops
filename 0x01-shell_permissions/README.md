<h2>Description</h2>
me is Betty

* Script that switches the current user to the user betty.



<table><tr><td>

#!/bin/bash

su betty

</td></tr></table>





1. Who am I

* Script that prints the effective username of the current user.



<table><tr><td>

#!/bin/bash

whoami

</td></tr></table>





2. Groups

* Sccript that prints all the groups the current user is part of.



<table><tr><td>

#!/bin/bash

groups

</td></tr></table>





3. New owner

* Script that changes the owner of the file hello to the user betty.



<table><tr><td>

#!/bin/bash

sudo chown betty hello 

</td></tr></table>





4. Empty!

* Script that creates an empty file called hello.



<table><tr><td>

#!/bin/bash

touch hello 

</td></tr></table>
------------------------
