# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
TippityTappity
  ExampleParent <|-- ExampleChild
  class ExampleParent{
        - Letters: string
        - Numbers: integer
        - Symbols: string
        + tpyingAccuracy(wpm: integer) boolean
        + get_wpm() integer
  }
  class ExampleChild{
        - wpm vector~integer~
        + add_wpm(title: string)
        + get_wpm() vector~integer~
  }
```
