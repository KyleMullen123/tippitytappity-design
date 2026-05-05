# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  ` User <|-- Ask_page
    note for User "can ask questions to mechanics"
    User <|-- Home_page
    User <|-- Login_page
    User  : +String name
    User  : +String question
    User  : +isvalid()
    User  : +answers()
    class Ask_page{
        +String question
        +ask()
        +answer()
    }
    class Login_page{
        -String user()
        -String password()
        -canLogin()
    }
    class Home_page{
        +bool is_login
        +home()
    }
```
