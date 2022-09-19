# Pars-OFF
This dataset is the first dataset for offensive detection in Farsi social media.
In this repository, we present the first dataset for offensive detection in Farsi social media.

The following is the demonstrates how to use Pars-OFF corpus associated files:

Pars-OFF corpus generally consists of 3 main parts:

Part 1 (Pars-OFF) consists of following files:
	Pars-OFF_all
	Pars-OFF_levela_train
	Pars-OFF_levela_test
	Pars-OFF_levelb_train
	Pars-OFF_levelb_test
	Pars-OFF_levelc_train
	Pars-OFF_levelc_test

Part 2 (Pars-OFF_ASPECT) consists of following files:
	Pars-OFF_aspect_train
	Pars-OFF_aspect_test
	Pars-OFF_aspect

Part 3 (Pars-OFF_KEY) consists of following file:
	Pars-OFF_KEY


Parts descriptions:

Part 1: in this part Pars-OFF corpus is categorized into 3 levels as described in main paper.
	Pars-OFF_all: first column is ‘tweet’ that contains tweet text, second is ‘level_a’ which can contain
	‘OFF’ and ‘NOT’ values. Third column is ‘level_b’ which can contain ‘TIN’, ‘UNT’ and NULL in case of 
	‘NOT’ in ‘level_a’ and Fourth column is ‘level_c’ that contains ‘IND’, ‘GRP’, ‘OTH’ and NULL in case of
	‘NOT’ in ‘level_a’ or ‘UNT’ in ‘level_b’.
	Pars-OFF_level*_train and Pars-OFF_level*_test: Each level of Pars-OFF corpus is divided into two 
	separate files of train and test, that train consists of 90% and test contains 10% of all the data.
	In each file, first column is ‘tweet’ that contains tweet text, and the second column is ‘label’ that 
	is the class of corresponding level.

Part 2: in this part targets of Level 3 of Pars-OFF corpus is  annotated. 
	Pars-OFF_aspect_train and Pars-OFF_aspect_test: These two files are corresponding with 
	Pars-OFF_levelc_train and Pars-OFF_levelc_test which all the targets are annotated as $Target$.
	Pars-OFF_aspect: for each annotated targets from level 3 of Pars-OFF_all, 3 lines are given. First 
	line consists of tweet that is related to target which target is replaced with $T$. At second line, 
	target is given and at third line, related label of level 3 is given.

Part 3: in this part Offensive and Abusive keyword in Persian is collected.
	Pars-OFF_KEY: In each line of this file an offensive keyword is given.

Please cite our paper in any published work that uses this resource.
