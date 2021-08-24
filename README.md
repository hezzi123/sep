# sep
def createX(number, s):
    feature = []
    for i in range(1, number):
        feature.append(f'{i}_' + s)
    feature.append(f'{number}_' + s)
    return feature

feature = createX(10, "Noradrenaline (Norepinephrine)") + createX(10, "ArtBPM") + createX(10, "LactateABG-1")
print(feature)
