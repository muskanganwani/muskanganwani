import os
import datetime
import time
n=1
c,b,a=input("Enter date =").split("/")
hr, minn , sec =input("Enter time =").split(":")
shedule_date =datetime.date(int(a),int(b),int(c))
while n>0:
    if time.localtime().tm_hour==int(hr) and time.localtime().tm_min==int(minn) and time.localtime().tm_sec==int(sec) and datetime.date.today()==shedule_date:
        os.startfile(r"C:\Users\HP\Music\Old_Alarm_Clock_Sound_-Ringing-Made_in_Germany_1920's-_30's.(128k).mp3")
        print("Alarm Ringing....")
        break
    else:
        n+=1
