# date14

with GNU date, date -d allows query such as 

`date -d "14 days ago"`

However using AIX date does not have this function.  For a legacy system witthout access to GNU date, we needed a way to check quickly and programmatically during validation.  This was written to be a functional equivalent to the above query and should continue to work until but not after 2099.  Dates after that time are expected to be outside the scope of its useful lifespan.

the script lives in .../lib/ and is meant to be called by other scripts as its return is an exit code.
