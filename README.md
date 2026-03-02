# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
TippityTappity
  Typing_Accuracy <|-- Typing_Speed
  class Typing_Accuracy{
        - Letters: string
        - Numbers: integer
        - Symbols: string
  }
  class Typing_Speed{
        - wpm vector~integer~
        + add_wpm(title: string)
        + get_wpm() vector~integer~
  }
```
