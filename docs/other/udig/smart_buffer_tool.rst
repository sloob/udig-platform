Smart Buffer Tool
#################

uDig : Smart Buffer Tool

This page last changed on Sep 21, 2012 by jgarnett.

Motivation
----------

Sometimes a user is working on a Polygon layer but only wants to draw a Point or line.

Inspiration
-----------

Converting a Point or Line to a Polygon usually involves applying a Buffer to the Point or Line, the
Point or Line line data must exist in a separate layer that supports the type of geometry, moving
the Buffered data over to your original Polygon layer can be a cumbersome process.

Proposal
--------

What if we can make use of the existing Point and Line tools and modify them to automatically apply
a buffer value to the Point or Line when working on a Polygon layer. The interactive PDF demo below
will demonstrate the idea in action.

NOTE, for the initial release I plan on only allowing users to modify the buffer value via the mouse
wheel and not via a field located in the Map status bar. This will be a future RFC and might be
generally useful for all tools. `Map Status Bar Tool
Options <Map%20Status%20Bar%20Tool%20Options.html>`__

Interactive PDF Demo
~~~~~~~~~~~~~~~~~~~~

| This is an interactive example, read the read text for instruction and click the Yellow link to
perform the action outlined by the instructions.
|  `Smart Buffer Tool
Example.pdf <download/attachments/13533810/Smart%20Buffer%20Tool%20Example.pdf>`__

-  If a point tool is selected and it is working on a Polygon layer the smart buffer will be
   activated.
-  If a point tool is selected and it is working on a point layer then a normal non buffered point
   will be drawn.
-  The amount of buffer can be adjusted using the mouse scroll wheel or via a form field.
-  A buffer value of greater than 0 must be used.

Status
------

Project Steering committee support:

-  Andrea Antonello: +1
-  Jesse Eichar: +1
-  Jody Garnett: +1
-  Mauricio Pazos: +1

Committer Support:

-  Kenneth Qulbrandsoy: +1

A vote of -1 requires an alternate suggestion; community members are invited to indicate
support/suggestions.

Documentation
-------------

Status
------

http://jira.codehaus.org/browse/UDIG-1811

Tasks
=====

A list of the tasks needed to accomplish this change; if you prefer you can use a single Jira issue
with subtasks. It is important to include any deadlines so the community knows when you are working
to a schedule.

 

no progress

|image0|

in progress

|image1|

blocked

|image2|

help needed

|image3|

done

Tasks RFC Process Sep 5-9th:

#. |image4| Initial interface wireframe for community review and feedback
#. Review deadline for RFC

Development Sep 12-15th:

#. |image5| Update point and line tool to apply buffer function only on polygon layer.
#. |image6| Allow buffer value to be changed via mouse wheel.
#. |image7| Allow buffer value to be changed in preference page.
#. |image8| Issue Pull Request
#. |image9| Updated user guide documentation

Tasks Friday 16 September

#. Accepted pull request, demo to customer at end of sprint, etc...

| 

Attachments:

| |image10| `Smart Buffer Tool
Example.pdf <download/attachments/13533810/Smart%20Buffer%20Tool%20Example.pdf>`__ (application/pdf)

+-------------+----------------------------------------------------------+
| |image12|   | Document generated by Confluence on Aug 11, 2014 12:31   |
+-------------+----------------------------------------------------------+

.. |image0| image:: images/icons/emoticons/star_yellow.gif
.. |image1| image:: images/icons/emoticons/error.gif
.. |image2| image:: images/icons/emoticons/warning.gif
.. |image3| image:: images/icons/emoticons/check.gif
.. |image4| image:: images/icons/emoticons/check.gif
.. |image5| image:: images/icons/emoticons/warning.gif
.. |image6| image:: images/icons/emoticons/check.gif
.. |image7| image:: images/icons/emoticons/check.gif
.. |image8| image:: images/icons/emoticons/check.gif
.. |image9| image:: images/icons/emoticons/star_yellow.gif
.. |image10| image:: images/icons/bullet_blue.gif
.. |image11| image:: images/border/spacer.gif
.. |image12| image:: images/border/spacer.gif
