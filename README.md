# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
TippityTappity
  TypingAccuracy <|-- TypingSpeed <|-- TypingHistory <|-- Montitor
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
  class TypingHistory{
        - Accuracy: string
        - Speed: integer
        + get_results(Accuracy: string, Speed: integer) booleana
  }
  class Montitor{
        - Users: string
        - History: string
        - Progress: string
        + get_history(Users: string, History: string, Progress: string) boolean
  }
```
