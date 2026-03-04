# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  TypingAccuracy <|-- TypingSpeed <|-- TypingHistory <|-- Montitor
  class TypingAccuracy{
        - Letters: string
        - Numbers: integer
        - Symbols: string
        + tpyingAccuracy(wpm: integer) boolean
        + get_wpm() integer
  }
  TypingSpeed{
        - wpm vector~integer~
        + add_wpm(title: string)
        + get_wpm() vector~integer~
  }
  TypingHistory{
        - Accuracy: string
        - Speed: integer
        + get_results(Accuracy: string, Speed: integer) booleana
  }
  Montitor{
        - Users: string
        - History: string
        - Progress: string
        + get_history(Users: string, History: string, Progress: string) boolean
  }
```
