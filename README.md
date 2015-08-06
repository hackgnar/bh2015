## Exercise 1
### Scenario:
You are testing out a new IP based network threat feed.  Determine all of the threat categories listed in the feed.  Which threat category is the most prevalent in this feed?

[Exercise 1 Threat Feed](https://github.com/hackgnar/bh2015/exercise_1_threat_feed.csv)

## Exercise 2
### Scenario:
You are provided with two IP based network threat feeds.  Determine the overlap (if any) between the two feeds.

[Exercise 2 Threat Feed 1](https://github.com/hackgnar/bh2015/exercise_2_feed_1.csv)

[Exercise 2 Threat Feed 2](https://github.com/hackgnar/bh2015/exercise_2_feed_2.csv)

## Exercise 3
### Scenario:
You have a sample network log and a sample threat feed list.  The entries in each file have already been labeled with an ingress/egress flag depending on the flow direction of the network connection of threat.  Using IP address and direction, determine how many alerts you would have in this small network data sample. 

[Exercise 3 Sample Network Data](https://github.com/hackgnar/bh2015/exercise_3_sample_network_data.csv)

[Exercise 3 Threat Feed](https://github.com/hackgnar/bh2015/exercise_3_threat_feed.csv)

## Exercise 4
### Scenario:
You have been provided with a sample list of threat feed alerts which have triggered in your environment.  The sample list is composed of target ip address and a description of the threat.  Use the provided passive DNS sample file to figure out how many domains have been seen for each IP address in your alerts.

[Exercise 4 Threat Feed Alerts](https://github.com/hackgnar/bh2015/exercise_4_threat_feed_alerts.csv)

[Exercise 4 Forward DNS Data](https://github.com/hackgnar/bh2015/exercise_4_foward_dns.csv)

## Hints
The linux ````comm```` command can be used to compare similar lines between two files.  Here is an example of how to use the command
```` bash
comm -12 file1.txt file2.txt
````

You can use ````awk```` to print a single column from a CSV.  The following example shows how:
```` bash
awk -F',' '{print $1}' file.csv
````

You can stream the results of a linux sub command though stdin to make it act as if your data is a file.  Here is an example:
```` bash
cat <(echo "how now brown cow")
````


