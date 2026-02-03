# JNSQ-OPM-Compatibility-Pack

# NOTE, THIS DOES ABSOLUTELY NOTHING EXCEPT MAKE EELOO COMPATIBLE, IT DOES NOT RESCALE THE PLANETS, CURRENTLY WORKING ON PATCH TO FIX THIS

For those who think JNSQ, GEP, and GPP together aren't enough planets

This allows for compatibility between JNSQ and OPM

I'm assuming you are capable of manual mod instalation, and I wouldn't reccomend using CKAN as CKAN will probably freak out that Eeloo.cfg doesn't exist inside OPM (idk, I don't use CKAN)

Dependancies are OPM and its dependancies, Sigma-Dimensions and its dependancies

to install, simply drag the GameData folder into the KSP install directory, or the contents of GameData into the KSP GameData folder
It will ask to replace some, hit yes.
Now you also need to navigate to OPM\KopernicusConfigs\SarnusMoons and delete Eeloo.cfg (it's a good idea to have a backup of OPM on hand if you want Eeloo to be a moon in a non-JNSQ save)

If you want to have Eeloo as a moon instead, you'll need to do that part yourself
basically delete all references to Eeloo inside JNSQ instead of OPM, and only use the rescale folder. You will need to add in these lines into the config to resize Eeloo
```
@Body[Eeloo]
{
  DoRescale = True
}
```
Planning on eventually adding a fork that does this for you, although that will take more time

If you have any mods that rely on the OPM planets, you will most likely need to go through them and remove references to Eeloo (mod confict testing has not and probably won't be tested by me)
