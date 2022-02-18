The things I like about my code:

1. The date initialization function 'python main.py init'. Instead of simply having a date in a text file, as the assignment suggests. This creates a new date, every time you run it. So even if you try the code again one year later, this again gives a current date, so you won't always have to work in last year. By using the timedelta's and the options to go back and forth between datetime objects and strings, the "day.csv" file is an important part.

2. The report function is a mostly a huge collection of if-statements, checking for different arguments. I'm glad it works well and that the argparser handles wrong input in the correct way. The function has gotten huge, because there are so many combinations of arguments possible. I chose to write it in this way to make the functionality versatile. The problem with it is that the code is so lang it becomes pretty unreadable. Is there any way in which I could have done this shorter?

3. In many occasions, I used the csv.DictReader and csv.DictWriter functions, instead of the csv.writer and csv.reader. This helps to for instance use line["product_name"] instead of line[2], which, even though it needs a bit more code, makes it more obvious to yourself and perhaps other reader what you're doing. I feel that by using the dict-functions, my code is less prone to errors.