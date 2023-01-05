# What can we do with football tracking data?

These data are the propriaty of Bepro and were transmitted thanks to Daniel Coppens.

Explanation of csv files below:

- TXT file is for the actual x, y positional data of all players and the ball, and XML file is for the metadata that explains the structure of the TXT file.
- There are 2 files in "XML" folder that we shared with you. bepro tracking data_FIRST_HALF.xml is related to bepro tracking data_FIRST_HALF.txt and bepro tracking data_SECOND_HALF.xml is related to bepro tracking data_SECOND_HALF.xml.

Basically, each row in TXT file represents the position of all 22 players and the ball, alongside the frame number and status of the ball. 
-> {frame number}:{player1's x},{player1's y};{player2's x},{player2's y}; ... ;{player22's x},{player22's y}:{ball's x},{ball's y}:{ball status}

From the sample row that you mentioned
261:9856,3349;6936,1441;7177,3118;7136,4182;6778,5861;6160,3347;6060,4184;5273,2481;5256,1890;5259,4362;5265,5018;5272,3418;5258,347;5254,6582;4394,2996;5184,4480;4435,3928;3637,1197;3442,2956;3380,3953;3652,5174;1066,3381:5252,3428:BALL_OUT
- 261: frame number
- 9856,3349: x, y coordinate of player 1 on the pitch at frame 261 (please use to the XML file to get team&player info)
- 6936,1441: x, y coordinate of player 2 on the pitch at frame 261
- ...
- 1066,3381: x, y coordinate of player 22 on the pitch at frame 261
- 5252,3428: x, y coordinate of the ball on the pitch at frame 261
- BALL_OUT: ball status at frame 261. There are 4 types of the ball status - BALL_OUT, HOME, AWAY, NEUTRAL based on the possession of the ball

Please note that frame number, player x&y coordinates, ball x&y coordinates and ball status are separated by colons.
