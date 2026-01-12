

## Project maken

- maak een nieuw Console project:
    - FileIo
- zorg dat je weer een Run function hebt


## File klaar zetten

- gebruik nu:
    - rechter muis op het project -> add
        > ![](img/nieuwtekst.PNG)
    - voeg een txt file toe
        - noem deze even quiz.txt

## File vullen

- kopieeer even de tekst van gamequestions.txt naar de quiz.txt
    - build & run het project
    - click op de `show all files` knop
        > ![](img/showfiles.PNG)
    - check of je nieuwe files ziet:
        > ![](img/hidden.PNG)
- open de bin
    > ![](img/bin.PNG)
    - zie je daar de quiz.txt staan?
        
## quiz.txt & copy

- in vscode:
- open je csproj file en zet het volgende erbij, ONDER <project>
```
<ItemGroup >
    <None Update="quiz.txt">
      <CopyToOutputDirectory>Always</CopyToOutputDirectory>
    </None>
    </ItemGroup>
```
- LETOP dit is voor Visual studio (2022+)
    - rechter muis op quiz.txt
        - properties
            - zet Copy to output ... naar Copy if newer:
                > ![](img/copy.PNG)

- build & run nogmaals
    - nu zie je quiz wel
        > ![](img/wel.PNG)
    
## commit

`commit` & `push` naar je git! 