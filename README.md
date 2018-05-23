# MLSA18 Football Pass Prediction Challenge

This repository contains the instructions and dataset for the Football Pass Prediction Challenge of the 5th Workshop on Machine Learning and Data Mining for Sports Analytics. The workshop will be held on Monday September 10th 2018 in Dublin as part of the European Conference on Machine Learning and Principles and Practice of Knowledge Discovery in Databases. Further information on the workshop is available on the [workshop website](https://dtai.cs.kuleuven.be/events/MLSA18/).

## Challenge

The goal of this challenge is to predict the receiver of a pass performed during a football match given the sender of the pass as well as the locations of all the players on the pitch. The focus of this challenge is on developing novel approaches to address this task.

## Dataset

The dataset contains 12,124 passes performed during 14 different games involving a Belgian football club during the 2014/2015 football season.

### Format

The `passes.csv` file contains the dataset in a comma-separated format. The file contains 12,125 rows and 60 columns. In addition to a header row, the file contains one row for each pass providing the following information:
- `time_start`: time elapsed in milliseconds since the start of the half at the time the ball was passed by the sender;
- `time_end`: time elapsed in milliseconds since the start of the half at the time the ball was received by the receiver;
- `sender_id`: the identifier of the player who passed the ball;
- `receiver_id`: the identifier of the player who received the ball;
- `x_*`: the x coordinates of the locations of the players on the pitch at the time of the pass;
- `y_*`: the y coordinates of the locations of the players on the pitch at the time of the pass.

### Identifiers

The players within each game are numbered from 1 till 28. Each team consists of 14 players: 11 starters and 3 substitutes. The players numbered from 1 till 14 belong to the home team, whereas the players numbered from 15 to 28 belong to the away team. Since the data were collected during different games involving different teams, the identifiers are only relevant within the scope of a single pass.

### Coordinates

The coordinates are expressed in centimeters in both directions of the pitch. The pitch is 105 meters long and 68 meters wide. The x-axis represents the long side of the pitch, whereas the y-axis represents the short side of the pitch:
- `(0, 0)`: center of the pitch;
- `(-5250, -3400)`: top-left corner of the pitch;
- `(-5250, 3400)`: bottom-left corner of the pitch;
- `(5250, -3400)`: top-right corner of the pitch;
- `(5250, 3400)`: bottom-right corner of the pitch.
 
## Contact

If you have any questions, suggestions or remarks, then please get in touch with Jan Van Haaren (j.vanhaaren@scisports.com). If you plan to participate in the challenge and submit a paper to the workshop, then please inform Jan Van Haaren as well. He will get in touch whenever any important information regarding the challenge would become available.
