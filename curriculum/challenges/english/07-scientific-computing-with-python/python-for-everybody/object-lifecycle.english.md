---
id: 5e7b9f170b6c005b0e76f087
title: Object Lifecycle
challengeType: 11
isRequired: true
videoId: p1r3h_AMMIM
---

## Description
<section id='description'>

</section>

## Tests
<section id='tests'>

```yml
question:
  text: |
    What will the following program print?:
    ```python
    class PartyAnimal:
        x = 0
        name = ''
        def __init__(self, nam):
            self.name = nam
            print(self.name,'constructed')
        def party(self):
            self.x = self.x + 1
            print(self.name,'party count',self.x)

    q = PartyAnimal('Quincy')
    m = PartyAnimal('Miya')

    q.party()
    m.party()
    q.party()
    ```
  answers:
    - |
        Quincy constructed

        Miya constructed

        Quincy party count 1

        Miya party count 2

        Quincy party count 3
    - |
        Quincy constructed

        Miya constructed

        Quincy party count 1

        Miya party count 1

        Quincy party count 2
    - |
        Quincy constructed

        Quincy party count 1

        Quincy party count 2

        Miya constructed

        Miya party count 1
  solution: 2
```

</section>
