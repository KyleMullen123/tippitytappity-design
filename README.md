# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
TippityTappity
  TypingAccuracy <|-- TypingSpeed
  class TypingAccuracy{
        - Letters: string
        - Numbers: integer
        - Symbols: string
        + tpyingAccuracy(wpm: integer) boolean
        + get_wpm() integer
  }
  class TypingSpeed{
        - wpm vector~integer~
        + add_wpm(title: string)
        + get_wpm() vector~integer~
  }
```
