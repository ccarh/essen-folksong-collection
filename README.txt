
       + + + + + + + + + + + + + + + + + + + + + + + + + + + + + + +
       +                                                           +
       +        THE ESSEN FOLKSONG COLLECTION IN KERN FORMAT       +
       +                                                           +
       +                     -  assembled by  -                    +
       +                                                           +
       +                    Dr. Helmut Schaffrath                  +
       +                                                           +
       +              Humdrum Kern version prepared by             +
       +                        David Huron                        +
       +                                                           +
       + + + + + + + + + + + + + + + + + + + + + + + + + + + + + + +


The Essen Folksong Collection is a database of some 6,255 folksong
transcriptions.  The collection consists primarily of folksongs from
Germany (5,370) and other Germanic regions -- Austria (104), Switzerland (93),
Alsace (91), Lothringen (71), the Czech Republic (43), and the Netherlands
(85).  The database also includes a handful of folksongs from other regions
of the world -- mostly European.  These include folksongs from Belgium (2),
Brazil (1), Canada (1), China (10), Denmark (9), Egypt (1), England (5),
Finland (1), France (14), Greece (1), Hungary (45), Iceland (2), India (1),
Ireland (1), Italy (8), Japan (1), Indonesia (1), Luxemburg (8), Mexico (4),
Norway (2), Poland (25), Romanian (28), Russia/USSR (37), Sweden (11), Syria
(1), Turkey (1), Ukraine (13), United States of America (7), Yugoslavia (119),
plus other miscellaneous works from regions such as Tirol, Steiermark,
Emmenthal, etc.  Of special note is a collection of 213 German Kinderlieder
(children's songs).

This large repository was assembled at the Gesamthochschule of Essen
University under the direction of Dr. Helmut Schaffrath.  The database was
developed from 1982 until Dr. Schaffrath's untimely death in 1994.

The continued development of this database is currently directed by
Dr. Ewa Dahlig at the Helmut Schaffrath Laboratory of Computer Aided
Research in Musicology, in Warsaw, Poland (eda@plearn.edu.pl), now at the
Polish Academy of Sciences in Warsaw, Poland.

Machine encoding, proof reading, and proof listening was done by, or
supervised by Dr. Schaffrath.  Preparation and editing of the Humdrum **kern
version was carried out by Dr. David Huron.  The database is published and
distributed by the Center for Computer Assisted Research in the Humanities.
Net proceeds after costs are donated to the Schaffrath Laboratory in Poland.
This electronic database is also available in the original Essen Associated
Code (ESAC) format.  (See below for ordering information.)

The accompanying files are protected by copyright and are distributed by
license only.  Refer to the accompanying license statement and original
license agreement for details.

========
CITATION
========

In cataloguing and publications, this database may by cited as follows:

    Schaffrath, Helmut
        The Essen Folksong Collection in Kern Format. [computer database]
        D. Huron (ed.).  Menlo Park, CA: Center for Computer
        Assisted Research in the Humanities, 1995.


============
ORGANIZATION
============

The collection is arranged as a series of directories according to
geographical region -- beginning with one of four continent designations
(Africa, America, Asia, Europa) followed by the country or region name.
In the case of Germany, further subdirectories are provided that
distinguish several different sources plus a separate directory for the
Kinderlieder.

All works are encoded in the Humdrum **kern format.  Refer to the accompanying
tutorial file ("kern_hlp.txt") for a detailed description of the **kern
representation.  All works consist of monophonic melodies.

============
INSTALLATION
============

The distribution disks are available only in DOS-format 1.44 megabyte
(3.5 inch) disks.  The database may be installed on UNIX, DOS, OS/2, or
Windows/NT systems.  The database is distributed via four disks containing
raw ASCII files.  For UNIX installations, a single compressed-format disk
is also available.  The compressed-format disk can also be installed
on DOS, OS/2, or Windows/NT systems that have access to the UNIX "uncompress"
utility.

The installation procedure is a two-part process.  The procedure is
currently not automated, and must be done manually by the user.

DOS or OS/2 INSTALLATION:
************************

PART ONE:

The first step is to copy all of the files into an appropriate directory
on your hard drive.

(1) Move to a directory where you would like to install the database.
    (Recommended: \scores\essen\)

(2) Insert the first distribution disk into an appropriate floppy disk drive.

    Copy all of the files from the distribution disk (including files in
    subdirectories) into the appropriate directory.  Assuming that the
    distribution disk is located in the A: drive, and that you wish to copy
    the files to the directory named \scores\essen,  the appropriate DOS
    or OS/2 command is:

         xcopy a: \scores\essen

(3) Insert each of the subsequent distribution disks, and repeat the
    xcopy command for each disk:

         xcopy a: \scores\essen

(4) When you have finished copying all of the distribution disks, continue
    to PART TWO (see below).

UNIX INSTALLATION:
******************

PART ONE:

The first step is to copy the files into an appropriate directory.

(1) Move to a directory where you would like to install the database.
    (Recommended: /scores/essen/)

(2) Recursively copy all of the files from the distribution disk into
    the appropriate directory.

    Assuming that the distribution disk is located in the A: drive,
    the appropriate UNIX command is:

         cp -r a:* /scores/essen

(3) Four directories should be present: africa, america, asia, europa.
    The vast majority of the files are in the "europa" directory --
    only the files in this directory are in compressed form.

    Change directories to "europa"

         cd europa

    There are 21 subdirectories:

    czech     danmark   deutschl  elsass    england   france    italia
    jugoslav  lothring  luxembrg  magyar    misc      nederlan  oesterrh
    polska    romania   rossiya   sverige   schweiz   ukraina   tirol

    For the moment ignore the "deutschl" directory.

    Each directory contain a file in compressed form (marked by the .Z
    extension in the filename).  Each .Z file must be uncompressed.  (If
    you are short of disk space you may want to maintain some files in
    compressed form.)

          NOTE:  DOS filenames are case-insensitive and so the .Z
          extensions may be rendered in lower-case (.z) on your
          system.  In order to uncompress the files, you may need
          to rename these files so that the .Z extensions are in
          upper-case.

    If you would like to uncompress all of the files, from the "europa"
    directory, execute the following command:

         uncompress */*

    (Ignore any error messages arising from subdirectories in the "deutschl"
    directory.)

(4) The "deutschl" directory contains the vast majority of folksongs.
    Under the directory "europa/deutschl" you will find the following
    subdirectories.

         allerkbd  altdeu1   altdeu2   ballad    boehme    dva      erk1
         erk2      fink      kinder    test      variant   zuccal

    Each of these subdirectory contains German folk songs from a different
    musicological source.  Change directories to the "deutschl" directory.
    Again, uncompress all of the sources by executing the following command
    from the "europa/deutschl" directory:

         uncompress */*

    Warning: The files in these directories will expand to approximately
    4 megabytes in size.


INSTALLATION: PART TWO  (DOS, OS/2 & UNIX)
**********************

Normally, Humdrum encodes each work in a separate file.  However DOS
format disks have difficulty storing thousands of small files.  As
a result, a single large file in each directory contains all of the
individual works concatenated together.  (Note that the Humdrum Toolkit
software can process the data in either form -- as a single large file,
or as individual files.)

For those users on UNIX systems or on DOS systems having installed the
Humdrum Toolkit, the concatenated files can be expanded into individual
files using the enclosed "expand.ksh" command.  To expand the files,
copy "expand.ksh" into the directory whose file you want to expand,
and type:

     expand <filename>        [on DOS]

     or

     chmod +x expand.ksh
     expand.ksh <filename>    [on UNIX]

N.B. The "expand" command will tell you how many new files will be
     created, and prompt you if you wish to abort.

==============
RESEARCH NOTES
==============

This **kern version of the Essen Folksong Collection was produced by
automated translation followed by hand editing.  A number of assumptions
were made in the production of this database and some of these assumptions
may confound certain scholarly uses.

 o The original database was encoded from a variety of sources;
   in most cases citations to sources were significantly abbreviated
   in the original ESAC data.  No attempt has been made to provide
   more complete reference information in this **kern translation.
   All citation information present in the source database has
   been retained; nevertheless, original sources may remain obscure.

 o The Essen Associative Code does not encode absolute pitch height.
   ESAC pitch information is represented by a combination of specifying
   the tonic pitch and giving (diatonic) solfege-type designations.
   In translating to **kern, it was necessary to estimate an appropriate
   octave placement.  For example, a work beginning on the mediant pitch
   with a tonic of C would need to be assigned to one of E3, E4 or E5, etc.
   In this **kern translation, the tonic pitch for the "principle octave"
   is assigned to the range C4-B4.

   In summary, although the relative pitch information and tonic is
   accurate, the absolute pitch-height information is unreliable
   in this database.

 o The **kern key designators require a distinction between major
   and minor keys -- information that was not present in the original
   ESAC databases.  Major/minor designations have been assigned
   according to the following (very simple) method:  keys were assumed
   to be major unless a lowered mediant or lowered submediant tone
   appeared in the first phrase -- in which case the key is assumed
   to be minor.  Note that many folksongs are best characterized as
   belonging to scales or modes other than major or minor.

   In summary, major/minor designations in this database are unreliable.

 o Note that the database contains a large number of folksongs that
   have been encoded with alternate renderings.  For example, more than 16
   variants of the German song "Muede kehrt ein Wandersmann" are encoded.
   For some statistical applications (such as in stylistics), such a high
   degree of repetition will violate assumptions of the independence
   of the works.

===============
REGIONAL NAMES:
===============

   Regional names in Humdrum encodings use Roman alphabet equivalents of
   the local language designations (e.g. Deutschland rather than Germany).
   The following table lists English equivalents and corresponding filenames
   for some of the regional names used in the Essen Folksong Collection.

       ENGLISH            LOCAL                FILENAMES

     Alsace       -     Elsass          -      elsass00
     Austria      -     Oesterreich     -      oester00
     Brazil       -     Brasil          -      brasil00
     Bulgaria     -     Bulgariya       -      bulgari0
     Croatia      -     Hrvatska        -      hrvatsk0
     Denmark      -     Danmark         -      danmark0
     Egypt        -     Misr            -      misr0000
     Finland      -     Suomi           -      suomi000
     Flanders     -     Vlaanderen      -      vlaandr0
     Germany      -     Deutschland     -      deut0000
     Greece       -     Ellas           -      ellas000
     Hungary      -     Magyar          -      magyar00
     Iceland      -     Island          -      island00
     Ireland      -     Eire            -      eire0000
     Italy        -     Italia          -      italia00
     Japan        -     Nippon          -      nippon00
     Netherlands  -     Nederland       -      neder000
     Norway       -     Norge           -      norge000
     Poland       -     Polska          -      polska00
     Russia       -     Rossiya         -      rossiya0
     Serbia       -     Srbija          -      srbija00
     Spain        -     Espana          -      espana00
     Sweden       -     Sverige         -      sverige0
     Syria        -     Ash Sham        -      ashsham0
     Switzerland  -     Schweiz, Suisse
                          Svizzera      -     schweiz/suisse00
     Turkey       -     Turkiye         -     turkiye00
     Yugoslavia   -     Jugoslavia      -     jugoslav0

======
INDEX:
======


The principal resources include 5,157 transcriptions of German folksongs
contained in eleven sub-directories.  The directory names reflect the
original names of the ESAC databases.

      Directory                 # of works              Files
      =========                 ==========              =====
      europa/deutschl/allerkbd     110        deut3663.krn to deut3772.krn
      europa/deutschl/altdeu1      309        deut3773.krn to deut4081.krn
      europa/deutschl/altdeu2      316        deut4082.krn to deut4397.krn
      europa/deutschl/ballad       687        deut2976.krn to deut3662.krn
      europa/deutschl/boehme       704        deut2272.krn to deut2975.krn
      europa/deutschl/dva          106        deut4398.krn to deut4503.krn
      europa/deutschl/erk1        1063        deut0567.krn to deut1629.krn
      europa/deutschl/erk2         642        deut1630.krn to deut2271.krn
      europa/deutschl/fink         566        deut0001.krn to deut0566.krn
      europa/deutschl/test          12        deut5146.krn to deut5157.krn
      europa/deutschl/variant       26        deut5120.krn to deut5245.krn
      europa/deutschl/zuccal       616        deut4504.krn to deut5119.krn
                                 =====
                    TOTAL         5157

A twelfth directory contains German children's songs:

      Directory                 # of works              Files
      =========                 ==========              =====
      europa/deutschl/kinder       213        kindr001.krn to kindr213.krn

                                 =====
             GERMAN TOTAL         5370

Twenty directories contain folksongs from other European nations:

      Directory                 # of works              Files
      =========                 ==========              =====
      europa/czech                  43        czech01.krn  to czech43.krn
      europa/danmark                 9        denmark1.krn to denmark9.krn
      europa/elsass                 91        elsass01.krn to elsass91.krn
      europa/england                 4        england1.krn to england4.krn
      europa/france                 14        france01.krn to france14.krn
      europa/italia                  8        italia01.krn to italia08.krn
      europa/jugoslav              119        jugos001.krn to jugos119.krn
      europa/lothring               70        lothr001.krn to lothr070.krn
      europa/luxembrg                7        luxemb01.krn to luxemb07.krn
      europa/magyar                 45        magyar01.krn to magyar45.krn
      europa/nederlan               85        neder001.krn to neder085.krn
      europa/oesterrh              104        oestr001.krn to oestr104.krn
      europa/polska                 25        poland01.krn to poland25.krn
      europa/romania                28        romani01.krn to romani28.krn
      europa/rossiya                37        ussr01.krn   to ussr36.krn
                                              rossiya01.krn
      europa/sverige                11        sverig01.krn to sverig11.krn
      europa/schweiz                93        swiss01.krn  to swiss93.krn
      europa/tirol                  14        tirol01.krn  to tirol14.krn
      europa/ukraina                13        ukrain01.krn to ukrain13.krn
      europa/misc                   30        emmenth1.krn to emmenth2.krn
                                              vlaandr1.krn to vlaandr2.krn
                                              island1.krn  to island2.krn
                                              norge01.krn  to norge02.krn
                                              oberhas1.krn to oberhas2.krn
                                              steier01.krn to steier11.krn
                                              appenzel.krn,   belgium1.krn
                                              brabant1.krn,   entlebug.krn
                                              ellas01.krn     eire01.krn,
                                              juedisch.krn    siebethl.krn
                                              suomi01.krn
                                 =====
NON-GERMAN EUROPEAN TOTAL          850

                                 =====
           EUROPEAN TOTAL         6220


Non-european repertoires include the following works:

      Directory                 # of works              Files
      =========                 ==========              =====

      africa                         1        arabic01.krn
      america/mexico                 4        mexico01.krn to mexico04.krn
      america/usa                    7        usa01.krn    to usa07.krn
      america/misc                   2        brasil01.krn,  canada01.krn
      asia/china                    10        china01.krn  to china10.krn
      asia/misc                      5        india01.krn,   nippon01.krn
                                              java01.krn ,   turkiye1.krn
                                              ashsham1.krn
                                 =====
       NON-EUROPEAN TOTAL           29

                                 =====
              GRAND TOTAL         6249


=========
FEEDBACK:
=========

Unlike printed musical scores, electronic editions are readily up-dated.
Should you encounter any errors in the enclosed data files, we'd like to
hear from you.  Your input can benefit other music scholars.  When re-
leasing subsequent electronic editions, our policy is to acknowledge by
name all users who identify unknown representation errors in our data.

