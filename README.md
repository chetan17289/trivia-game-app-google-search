# Trivia app game Google search script

A simple python script to Google search the trivia app game question and find the probablity of correctness of each options.

## Dependencies
- Python 3
- Pyscreenshot
- Tessaract OCR
- BeautifulSoup
## How it works?
The script when executed, takes the screenshot, marked by the coordinates of the screen, and then use TessaractOCR to extract the questions and the options. The questions is search on Google and then probablity of correctness of each option is calculated using the frequency of occurence of options.

## How to run?
- Mirror or run the App on your PC
- Set the coordinates of the question at 
```imq = ImageGrab.grab(bbox=(X1, Y1, X2, Y2))```
- Similarly, set the coordinates of each options
```python
imo1 = ImageGrab.grab(bbox=(X1, Y1, X2, Y2)) #Option 1
imo2 = ImageGrab.grab(bbox=(X1, Y1, X2, Y2)) #Option 2
imo3 = ImageGrab.grab(bbox=(X1, Y1, X2, Y2)) #Option 3
```

- Run the script using ```python3 script.py``` when question appears on the screen.
