# dev-utils
Tools to help you develop


## TextSet

### usage)
```bash
python TextSet.py \
'
red
green
blue
' \
'
black
red-mango
green
'
```

### output)
```
########### Set A ################	//
blue
green
red
########### Set B ################	//
black
green
red-mango
########### A - B ################	//
blue
red
########### B - A ################	//
black
red-mango
########### A and B ################	//
green
########### A or B ################	//
black
blue
green
red
red-mango
########### (A or B) - (A and B) ################	//
black
blue
red
red-mango
```
