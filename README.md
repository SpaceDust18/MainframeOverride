claudiabolivar@Claudias-MacBook-Pro Unit4.MainframeOverride % psql
Password for user claudiabolivar: 
psql (17.4)
Type "help" for help.

claudiabolivar=# \l
                                                        List of databases
        Name        |     Owner      | Encoding | Locale Provider | Collate | Ctype | Locale | ICU Rules |   Access privileges   
--------------------+----------------+----------+-----------------+---------+-------+--------+-----------+-----------------------
 claudiabolivar     | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 mainframe_override | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 pit_stop           | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 postgres           | postgres       | UTF8     | libc            | C       | C     |        |           | 
 template0          | postgres       | UTF8     | libc            | C       | C     |        |           | =c/postgres          +
                    |                |          |                 |         |       |        |           | postgres=CTc/postgres
 template1          | postgres       | UTF8     | libc            | C       | C     |        |           | =c/postgres          +
                    |                |          |                 |         |       |        |           | postgres=CTc/postgres
(6 rows)

claudiabolivar=# \c mainframe_override;
You are now connected to database "mainframe_override" as user "claudiabolivar".
mainframe_override=# \l
                                                        List of databases
        Name        |     Owner      | Encoding | Locale Provider | Collate | Ctype | Locale | ICU Rules |   Access privileges   
--------------------+----------------+----------+-----------------+---------+-------+--------+-----------+-----------------------
 claudiabolivar     | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 mainframe_override | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 pit_stop           | claudiabolivar | UTF8     | libc            | C       | C     |        |           | 
 postgres           | postgres       | UTF8     | libc            | C       | C     |        |           | 
 template0          | postgres       | UTF8     | libc            | C       | C     |        |           | =c/postgres          +
                    |                |          |                 |         |       |        |           | postgres=CTc/postgres
 template1          | postgres       | UTF8     | libc            | C       | C     |        |           | =c/postgres          +
                    |                |          |                 |         |       |        |           | postgres=CTc/postgres
(6 rows)

mainframe_override=# \dt
                   List of relations
 Schema |        Name         | Type  |     Owner      
--------+---------------------+-------+----------------
 public | emptystack_accounts | table | claudiabolivar
 public | forum_accounts      | table | claudiabolivar
 public | forum_posts         | table | claudiabolivar
(3 rows)

mainframe_override=# SELECT * FROM forum_posts;
  id   |                                             title                                              |                                                                                                                        content                                                                                                                        |          date           |              author               
-------+------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------+-----------------------------------
 7wCbt | Tui certus colo absque deprimo deinde utroque.                                                 | Acsi vicinus tamdiu dolor tabula concido cuius termes. Statim vilitas tam. Utilis tutis temeritas.                                                                                                                                                    | 2049-11-01 21:03:23.181 | slimy-elver-53
 yUtle | Sit quos subito sopor coruscus at.                                                             | Possimus velit accusamus. Suscipit alius officia amor carmen ratione. Adipiscor coma utor stabilis qui optio vulnus.                                                                                                                                  | 2046-12-07 05:02:49.874 | experienced-import-25
 HKSjw | Molestias vestrum articulus concedo surgo stillicidium facilis victoria tyrannus.              | Verbum aedificium vacuus cado toties argentum pauci ventosus clamo alter. Varius ventosus dolorum. Circumvenio tenus tempus.                                                                                                                          | 2049-07-21 22:59:11.974 | neglected-chow-92
 y9i7r | Demoror confugo suppellex depono vester annus tenuis tristis apostolus vero.                   | Voluptatum caries fugiat. Tersus ullam amissio. Utrimque convoco amplus valde comprehendo.                                                                                                                                                            | 2048-12-04 19:40:00.281 | hidden-filter-93
 mx_WA | Illo urbanus tunc conqueror cogito tamisium quis aequus.                                       | Harum theologus complectus alius administr
  id   |                                      title                                       |                                                                                              content                                                                                               |          date           |           author           
-------+----------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------+----------------------------
 jnB2t | Depraedor casus arcus vitium statua labore sequi comitatus corrigo amitto.       | Deludo alter totidem arx crudelis campana qui. Denuncio corporis totidem tutis aer animi commodo. Amet sulum contra aperte coerceo civitas tergiversatio. dad                                      | 2048-04-03 06:07:19.384 | corny-disclosure-70
 RjiqA | Altus clarus pectus amplitudo.                                                   | Balbus tabula custodia veniam. Utor ciminatio tergum vado accedo uterque pectus suppellex nobis maxime. Talio cavus sustineo copia coniuratio odio arbitro suscipio. dad                           | 2048-04-25 02:55:18.124 | well-off-opera-35
 1Rj_j | Conitor comedo corporis illo depereo adopto cervus tribuo vere.                  | Thorax timidus audeo sodalitas. Comis appono comis utilis. Tristis cubitum volup varietas aliquid vindico attonbitus vix decet.                                                                    | 2048-04-23 10:13:06.935 | definite-ecliptic-82
 LinS6 | Amicitia cultura velit ocer votum contego solus videlicet coniuratio molestias.  | Comptus utilis usque torrens benevolentia ultio. Venia iste taceo summisse aufero viduo cilicium. Victoria sodalitas demum.                                                                        | 2048-04-11 03:15:16.632 | somber-cook-47
 pkNp7 | Argentum cubitum patrocinor totus utroque deleo temperantia.                     | Aureus depono constans nisi sophismata pax teneo animadverto. Quis timor cunctatio unus accendo nisi aeneus vado censura. Thorax arx illum adaugeo tempus cras. EmptyStack                         | 2048-04-02 12:50:36.588 | steep-mechanic-65
 EAPZ0 | Abundans validus advenio audax.                                                  | Theca varietas consequuntur triumphus adsuesco suppellex virgo antiquus amet suscipit. Delinquo caecus vesica spes aureus appositus vomer. Aedificium vicissitudo defendo solum video. dad         | 2048-04-24 09:57:14.81  | whispered-brochure-38
 nbZY_ | Get rich fast                                                                    | You should all invest in EmptyStack Solutions soon or you'll regret it. My dad works there and he's got some serious inside intel. Their self-driving taxis are the future and the future is here. | 2048-04-08 00:00:00     | smart-money-44
 YD6j0 | Vinum nemo varietas.                                                             | Tenax tenax ancilla cultura surculus ceno verecundia cavus tui. Subiungo velum adipisci. Clibanus considero cohibeo
mainframe_override=# SELECT * forum_accounts WHERE username = 'smart-money-44';
ERROR:  syntax error at or near "forum_accounts"
LINE 1: SELECT * forum_accounts WHERE username = 'smart-money-44';
                 ^
mainframe_override=# SELECT * FROM forum_accounts WHERE username = 'smart-money-44';
    username    | first_name | last_name 
----------------+------------+-----------
 smart-money-44 | Brad       | Steele
(1 row)

mainframe_override=# SELECT * FROM emptystack_accounts WHERE last_name = 'Steele';
    username    |  password   | first_name | last_name 
----------------+-------------+------------+-----------
 triple-cart-38 | password456 | Andrew     | Steele
 lance-main-11  | password789 | Lance      | Steele

 mainframe_override=# \dt
                   List of relations
 Schema |        Name         | Type  |     Owner      
--------+---------------------+-------+----------------
 public | emptystack_accounts | table | claudiabolivar
 public | emptystack_messages | table | claudiabolivar
 public | emptystack_projects | table | claudiabolivar
 public | forum_accounts      | table | claudiabolivar
 public | forum_posts         | table | claudiabolivar
(5 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE content LIKE '%self-driving%';
ERROR:  column "content" does not exist
LINE 1: SELECT * FROM emptystack_messages WHERE content LIKE '%self-...
                                                ^
mainframe_override=# SELECT * FROM emptystack_messages;
  id   |              from              |       to       |                                         subject                                         |                                                                                                                 body                                                                                                                 
-------+--------------------------------+----------------+-----------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 lmtdv | any-role-69                    | triple-cart-38 | Absque defero abundans thymbra vinitor tenetur.                                         | Vesco assentator tondeo defetiscor ver adversus agnitio usitas deprimo aveho. Agnosco adhaero derelinquo absconditus vobis. Venustas terminatio balbus amor tabernus currus corrigo.
 RXehN | measly-concentration-28        | triple-cart-38 | Sursum studio circumvenio demoror comprehendo.                                          | Vapulus valetudo censura supellex cuppedia. Ter adiuvo armarium alveus voluptates. Conitor valde dens alius brevis cognomen sumptus debilito.
 SL2Ph | puzzled-overheard-86           | triple-cart-38 | Statua copiose vincul
  id   |              from              |       to       |                      
                   subject                                         |            
                                                                                
                     body                                                       
                                                          
-------+--------------------------------+----------------+----------------------
-------------------------------------------------------------------+------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
----------------------------------------------------------
 lmtdv | any-role-69                    | triple-cart-38 | Absque defero abundan
s thymbra vinitor tenetur.                                         | Vesco assen
tator tondeo defetiscor ver adversus agnitio usitas deprimo aveho. Agnosco adhae
ro derelinquo absconditus vobis. Venustas terminatio balbus amor tabernus currus
 corrigo.
 RXehN | measly-concentration-28        | triple-cart-38 | Sursum studio circumv
enio demoror comprehendo.                                          | Vapulus val
etudo censura supellex cuppedia. Ter adiuvo armarium alveus voluptates. Conitor 
valde dens alius brevis cognomen sumptus debilito.
mainframe_override=# SELECT * FROM emptystack_messages WHERE body LIKE '%self-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE subject LIKE '%self
-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE body ILIKE '%self-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# \d
                   List of relations
 Schema |        Name         | Type  |     Owner      
--------+---------------------+-------+----------------
 public | emptystack_accounts | table | claudiabolivar
 public | emptystack_messages | table | claudiabolivar
 public | emptystack_projects | table | claudiabolivar
 public | forum_accounts      | table | claudiabolivar
 public | forum_posts         | table | claudiabolivar
(5 rows)

mainframe_override=# \d emptystack_messages
       Table "public.emptystack_messages"
 Column  | Type | Collation | Nullable | Default 
---------+------+-----------+----------+---------
 id      | text |           | not null | 
 from    | text |           | not null | 
 to      | text |           | not null | 
 subject | text |           | not null | 
 body    | text |           | not null | 
Indexes:
    "emptystack_messages_pkey" PRIMARY KEY, btree (id)

mainframe_override=# SELECT * FROM emptystack_messages WHERE body ILIKE '%self-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE body ILIKE '%self-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE subject ILIKE '%self-driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE body ILIKE '%driving%';
 id | from | to | subject | body 
----+------+----+---------+------
(0 rows)

mainframe_override=# SELECT * FROM emptystack_messages WHERE body ILIKE '%taxi%';
  id   |     from     |       to       |   subject    |                            body                            
-------+--------------+----------------+--------------+------------------------------------------------------------
 LidWj | your-boss-99 | triple-cart-38 | Project TAXI | Deploy Project TAXI by end of week. We need this out ASAP.
(1 row)

mainframe_override=# SELECT * FROM emptystack_accounts WHERE username = 'your-boss-99';
   username   |    password    | first_name | last_name 
--------------+----------------+------------+-----------
 your-boss-99 | notagaincarter | Skylar     | Singer
(1 row)

mainframe_override=# \d emptystack_projects
       Table "public.emptystack_projects"
 Column | Type | Collation | Nullable | Default 
--------+------+-----------+----------+---------
 id     | text |           | not null | 
 code   | text |           | not null | 
Indexes:
    "emptystack_projects_pkey" PRIMARY KEY, btree (id)

mainframe_override=# SELECT * FROM emptystack_projects WHERE code = 'TAXI';
    id    | code 
----------+------
 DczE0v2b | TAXI
(1 row)

mainframe_override=# \q
claudiabolivar@Claudias-MacBook-Pro Unit4.MainframeOverride % node mainframe -st
op
WARNING: admin access required. Unauthorized access will be logged.
Username: your-boss-99
Password: notagaincarter
Welcome, your-boss-99.
Project ID: DczE0v2b
Initiating project shutdown sequence...
5...
4...
3...
2...
1...
Project shutdown complete.
claudiabolivar@Claudias-MacBook-Pro Unit4.MainframeOverride % 