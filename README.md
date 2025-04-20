# datetime
# greet_by_time.py

from datetime import datetime

def greet():
    now = datetime.now()
    hour = now.hour

    if hour < 12:
        greeting = "Good morning! ☀️"
    elif 12 <= hour < 18:
        greeting = "Good afternoon! 🌤️"
    else:
        greeting = "Good evening! 🌙"

    print(f"{greeting} The current time is {now.strftime('%H:%M')}.")

if __name__ == "__main__":
    greet()
