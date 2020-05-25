# epoch
The time module provides a function, also named time, that returns the current Greenwich Mean Time in “the epoch”, which is an arbitrary time used as a reference point. On UNIX systems, the epoch is 1 January 1970.  >>> import time >>> time.time() 1437746094.5735958 Write a script that reads the current time and converts it to a time of day in hours, minutes, and seconds, plus the number of days since the epoch.

import time

epoch=time.time()

   
def epoc(t):
    tdias=int (t//86400)
    horas=int((t%86400)/3600)
    minutos=int((t%3600)/60)
    segundos=int((t%60))
    print(horas,':',minutos,':',segundos,' numero de dias desde epoch',tdias)
    
epoc(epoch)
