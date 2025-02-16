The Opaque question type and behaviour

Opaque (http://docs.moodle.org/en/Development:Opaque) is the
Open protocol for accessing question engines.

The Opaque protocol was originally created by sam marshall of
the Open University (http://www.open.ac.uk/) as part of the
OpenMark project (http://java.net/projects/openmark/).
The Moodle implementation of Opaque was done by Tim Hunt.

As well as OpenMark, this question type can also be used to
connect to STACK (http://www.stack.bham.ac.uk/) and possibly
other question systems we don't know about.


Opaque has been available since Moodle 1.8, but this version is
compatible with Moodle 2.1+. (For older versions, see
http://cvs.moodle.org/contrib/plugins/question/type/opaque/.)

This question behaviour also requires the Opaque question type
to be installed.

To install using git, type this command in the root of your Moodle install
    git clone git://github.com/timhunt/moodle-qtype_opaque.git question/type/opaque
    git clone git://github.com/timhunt/moodle-qbehaviour_opaque.git question/behaviour/opaque
Then add question/type/opaque and question/behaviour/opaque to your git ignore.

Alternatively, download the zip from
    https://github.com/timhunt/moodle-qtype_opaque/zipball/master
unzip it into the question/type folder, and then rename the new
folder to opaque. Then download the zip
    https://github.com/timhunt/moodle-qbehaviour_opaque/zipball/master
unzip it into the question/behaviour folder, and then rename the new
folder to opaque.


Once installed you need to go to the question type settings page
(Site administration -> Plugins -> Question types -> Opaque) to
set up the URLs of the question engines you wish to use.
