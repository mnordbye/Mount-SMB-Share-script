#!/bin/bash

# Script for connecting to a selection of SMB shares in order.
# Checks for connection first, then connects.
#
# Magnus Nordbye 2022.


# Find name of logged in user

loggedInUser=$( scutil <<< "show State:/Users/ConsoleUser" | awk '/Name :/ && ! /loginwindow/ { print $3 }' )

# Connect to shares. Add more "else" arguments to add more shares to the script.

if ping -c1 {insert IP/DNS name here}
then
  open "smb://${loggedInUser}@{insert IP/DNS name here}"
elif ping -c1 {insert IP/DNS name here}
then
  open "smb://${loggedInUser}@{insert IP/DNS name here}"
else
  open "smb://${loggedInUser}@{insert IP/DNS name here}"
fi

exit 0
