Burlap source: http://burlap.cs.brown.edu/
Template source: https://github.com/juanjose49/omscs-cs7641-machine-learning-assignment-4/blob/master/LICENSE
GitHub Link: https://github.com/tobincolby/CS4641-MDP

To produce the data and graphs used in the analysis (on a bash terminal):
	Enter the root of the Code directory and execute `mvn compile`
	Then, run: 

		for i in 0 1 2 
		do
			for j in 0 1 2 
			do
				mvn exec:java -Dexec.mainClass="assignment4.EasyGridWorldLauncher" -Dexec.args="$i $j"
				mvn exec:java -Dexec.mainClass="assignment4.HardGridWorldLauncher" -Dexec.args="$i $j"
			done
		done


The above will produce all required data on stdout and will create pop-up windows for all policy graphs

