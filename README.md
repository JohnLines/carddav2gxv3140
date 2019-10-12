# carddav2gxv3140

This program takes a CardDAV phone book (currently using khard
to generate it), and converts it into a phonebook.xml suitable
for being downloaded by a Grandstream GXV3140 SIP phone.

Set up and configure khard to extract data from all the CardDAV
address books you use, such that 'khard phone' will give you
a list of people and phone numbers.

The phone numbers are extracted and converted and stored in
~/.local/share/carddav2html/carddav-phonebook.xml

This is compared with the master file at
/var/www/html/phonebook.xml

but if the two are different the program only show the
differences, and does not update the master file.

If the differences are valid then the created file should
be manually copied to the master file.

