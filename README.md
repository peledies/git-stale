git-stale
=========

A Git extension for listing branches sorted by their last commit date in a column view with some color prettification

###Install instructions

Clone the script to your current working directory
<pre>$ git clone https://github.com/peledies/git-stale.git</pre>

Move the script to a location that is in your environment path
<pre>$ sudo cp git-stale/git-stale /usr/local/bin/git-stale</pre>

###Usage
From a current git project issue the following command
<pre>$ git stale</pre>

####Optional Argument
An optional argument can be added to git-stale to grep the output for matches. So if you wanted to only show branches created by a specific user then 
you could pass the users name, or if you wanted to search for a branch that had a certain text in its name you could pass that text.
<pre>$ git stale John</pre>

###Troubleshooting
If the script is not found it is most likely that you dont have /usr/local/bin set up in your environmental path variable
look at your bash profile and ensure that there is a line like the following in there

<pre>export PATH=/usr/local/bin:$PATH</pre>

There may be additional paths in there as well. Thats ok. Just make sure /usr/local/bin is in there as well.
You will need to re-source your bash profile if you do edit it by issuing the following command
<pre>$ source ~/.bash_profile</pre>


