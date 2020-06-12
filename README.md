# Git på svenska

## Introduktion

Detta är en fork av [git-pa-svenska](https://github.com/bjorne/git-pa-svenska).
Idé från [bjorsa](https://github.com/bjorsa)

Den har utifrån samma utgångspunkt att försöka hitta ett sätt att kunna kommunicera 
på svenska det man gör i git. 

Från git-pa-svenska](https://github.com/bjorne/git-pa-svenska): 
*Det dagliga språket för de olika kommandona i `git` (eller `jävel`) är
på svenska ett enda stort svengelskakalas. Jag finner mig själv ofta
sägandes _"Kan du pusha branchen?"_ eller _"Jag pullar!"_, vilket
känns pinsamt.*

Detta dokument utgör ett alternativ till git-pa-svenska](https://github.com/bjorne/git-pa-svenska) 
för att förhoppningsvis göra det än lättare att kommunicera. 

Termerna kommer från: [sjotermer](http://omk.se/anslagstavlan/sjotermer)

## Förslag

Nedan följer tabeller över verb och substantiv relaterade till git,
deras nuvarande bruk samt förslag på hur vi tillsammans kan bättra
oss.

| Verb        | Nuvarande bruk | Förslag       |
|-------------|----------------|---------------|
| pull        | pulla          | lägga-till    |
| push        | pusha          | lägga-ut      |
| fetch       | fetcha         | hala-hem      |
| branch      | brancha        | rutt          |
| commit      | commita        | förankra      |
| rebase      | rebasa         | brassa        |
| merge       | merga          | anlöpa        |
| squash      | squasha        | knopa (-ihop)  |
| stash       | stasha         | ?????         |
| tag         | tagga          | märke         |
| cherry-pick | cherry-picka   | plocka???     |
| amend       | amenda         | ?????         |
| blame       | blamea         | kölhala       |

| Substantiv   | Nuvarande bruk | Förslag           |
|--------------|----------------|-------------------|
| git          | git            | gigg              |
| repository   | repo           | durk/holk         |
| branch       | branch         | rutt              |
| commit       | commit         | förankring        |
| pull request | pull request   | angörningsfråga   |
| stash        | stash          | ?????             |
| tag          | tagg           | märka             |

## Exempel

    - Kan du lägga-till rutten jag just brassade och lägga-ut till github?

    - Jag la nyss en ny rutt och förankrade ändringarna från min durk där.

    - Skicka en angörningsfråga när du är anlöpt!

    - Låt oss plocka från huvud-rutten.
    
    - Hoppsan, jag råkade visst kraft lägga-till mot huvud-rutten.. D:

    - Knopa ihop dina förankringar innan du anlöper.

## Dagligt bruk

Nedan följer en rad kommandoradskommandon för att sätta upp en svensk
gitmiljö. Avsaknaden av svenska tecken i täcknamnen beror på en brist i git
(överväg att förbättra mjukvaran och skicka en ryckbegäran!). Följande
kommandon ändrar din `~/.gitconfig` och kommer att verka globalt.

    git config --global alias.lagga_till pull
    git config --global alias.lagga_ut push
    git config --global alias.rutt branch
    git config --global alias.forankra commit
    git config --global alias.brassa rebase
    git config --global alias.anlopa merge
    git config --global alias.durk stash
    git config --global alias.kolhala blame
    git config --global alias.marke tag
    git config --global alias.mark tag

    alias gigg=git
