`arc-inventory`
displays all the AWS resources represented by the cwd .arc file

`arc-inventory verify`
check for existence of AWS resources based on the cwd .arc file

`arc-inventory nuke`
delete all resources defined by .arc except dynamodb tables

`ARC_NUKE=tables arc-inventory nuke`
delete ONLY dynamodb tables

TODO
- `arc-inventory verify` should warn about orphaned resources
  - lambda functions
  - dynamodb tables
  - sns topics
- `arc-inventory clean` remove orphaned resources
