# CountDown
#simple  birthday Countdown
import time
def  countdown(t):
    while t:
        mins, secs=divmod(t, 60)
        timer ='{:02d}:{:02d}'.format(mins, secs)
        print(timer, end="\r")
        time.sleep(1)
        t=t- 1
    print("hHEYYY ITS YOUR BIRHDAYY !!")
    print("   HAPPY BIRTHDAY.....")
t = input("Few seconds to go: ")
countdown(int(t))
