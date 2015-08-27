# MultiplesInstanciasText

 ** revisar cat /etc/oratab  ***

1. dbca( for Database Configuration Assistent).
2. delete database in "Database Configuration Assistent"

#Verificar que se hallan borrado las instancias en /u01/app/oracle/orada/

**Create a new database whith Database Configuration Assistent**


*Note : 
1. Activate sample schemas
2. Location Default 
3. Flash recovery area default
4. Memory of 1024 aprox. Because the memory is comparted;
5. Next to steep 11 and Create a database
6. Select port of the new database

**Example https://servidor32:5500/em**
**Example https://servidor32:5501/em**



verificar con netstat -na

verificar echo $ORACLE_SID (verificar instancia);

change of instancia : ORACLE_SID="nueva instancia" y despues verificas con echo $ORACLE_SID;

verificar en oracle´s shell with select instance_name from v$instance;

Nota "startup listener for all instances" then
emctl  start dbconsole (Enterprise manager) this is one by one intances created;
check browser all conections of instances;
warning : not close enterprise with out logon off of the session

and now shutdown all
first lsnrctl stop 
second emctl stop dbconsole

if you erase a default instance you change in a bash profile ORACLE_SID;
cd nano .bash_profile
EDIT ORACLE_SID
then logout of the session oracle and login again;




