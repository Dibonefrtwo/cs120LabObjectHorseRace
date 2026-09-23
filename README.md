# cs120LabObjectHorseRace
BSU CS 121 course: lab 4

## Horse::Horse()
```
set position to 0 
set index to 0 
set trackLength to 15 
```
## void Horse::init(int index, int tracklength)
``` 
set position to 0 
set Horse::index to index 
set Horse::trackLength to trackLength 
```

## void Horse::advance()
```
assume random generator is seeded (maybe in race)
temp int gets random int (0/1)
add temp int to Horse::position
```

## void Horse::printLane()
```
make for loop, pos goes from 0 to trackLength 
  if pos == Horse::position:
    print Horse::index
  else 
   print '. '
after loop print newLine
```

## bool Horse::isWinner()
```
bool result = false 
if position >= trackLength 
 result = true
 print some commentary  
return result
```

## Race::Race()
```
const static int NUM_HORSES = 5 
const in TRACK_LENGTH = 15 

seed random generator 

initialize the horse array 
for each horse: 
  initialize with index and trackLength 
```

## void Race::start()
``` 
bool keepGoing = trye 
while keepGoing 
  for each horse: 
   advanace horse 
   print lane horse 
   isWinner horse 
    if winner keepGoing false
```
