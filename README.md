# project
fake news generator
#import the random module
import random

# create subjects:
subjects = [
    "delhi highway",
    "car",
    "waterfall",
    "truck",
    "highway",
    "four men ",
    "virtus"
]
actions = [
    "accident",
    "beaten",
    "fight",
    "dance",
    "fests"

]
places= [
    "college",
    "school",
    "highway",
    "delhi",
    "dwarka",
    "nsut"
]
# start the headline generation loop
while True:
    subject = random.choice (subjects)
    action = random.choice(actions)
    places = random.choice(places)

    headline = f"BREAKING NEWS: {subject} {action } {places}"
    print("\n" + headline)

    userinput =  input("\n do you want to generate new headline? (yes/no)").strip()
    if userinput == "no":
        break

    print("\n thanks for using this fake news generator system, have a great day")
