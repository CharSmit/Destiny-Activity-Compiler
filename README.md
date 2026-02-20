# Destiny Activity Compiler
Command line program designed to compile all the activities ever completed by a player, and output it to activities.csv file
This is a program designed to be later implemented into an application, however it works as a standalone. can be run using ./tracker in terminal, however if you wish to compile it with your personal API key the command
 g++ tracker.cpp -o tracker -lcurl -DBUNGIE_API_KEY="\"your_key_here\""
 will do that.
 The output contains the date of the activity, the time it took, and a link to the pgcr on the official bungie.net, a version containing a GUI and additional details will be created later.
 to retrieve the data of a user type in their bungie name and id, an example is provided
