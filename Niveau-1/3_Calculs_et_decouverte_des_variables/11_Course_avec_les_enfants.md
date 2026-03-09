# 11. Course avec les enfants

<img src="ressources/schema.png">

Le Robot doit faire en sorte de prendre les anneaux puis de les déposer derrière la ligne rouge à gauche il ne peut prendre qu'un seul anneu à la fois !

```Java
import static algorea.Robot.*;

class Main {

  public static void main(String[] args) {
    int nbMarche = 1;
      for(int i = 0; i < 10; i++){
        for(int x = 0; x < nbMarche; x++) {
          droite();
        }
        ramasser();
        for(int y = 0; y < nbMarche; y++) {
          gauche();
        }
        deposer();
        nbMarche++;
      }
  }
}
```
