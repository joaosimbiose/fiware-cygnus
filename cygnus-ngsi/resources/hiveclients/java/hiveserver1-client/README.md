#HiveServer1 client

##Installation and run
Build the Hive basic client with Maven:

    $ cd resources/hiveclients/java/hiveserver1-client
    $ mvn package

You can run the built application by using Maven too (please observe with HiveServer1 the initial database is always the default one):

    $ mvn exec:java -Dexec.args="<hive_host> <hive_port> <hadoop_user> <hadoop_password>"

Once it is running, you will see a prompt asking you for HiveQL sentences to be executed:

    remoteclient>

You can write any set of HiveQL sentences separated by `;`, for instance:

    remoteclient> select * from <table>;
    [data_being_printed]

Type `exit;` for closing the client.

##Contact

Francisco Romero Bueno (francisco.romerobueno@telefonica.com)
<br>
Fermin Galán Márquez (fermin.galanmarquez@telefonica.com)
