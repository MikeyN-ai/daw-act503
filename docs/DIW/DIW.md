# II. Disseny d'interfícies Web

## II.1. Resum general

Hem finalitzat la maquetació i integració de les diferents seccions, tant estàtiques com dinàmiques, dels projectes **Selectio** i **Nexapp**. A més de completar la part pública de les dues aplicacions, també hem desenvolupat i millorat els respectius **backoffice**, permetent la gestió de continguts, usuaris i dades de manera més eficient.

També hem revisat aspectes relacionats amb la navegació, la usabilitat i el disseny responsive per tal de garantir una bona experiència d'usuari en diferents dispositius.

## II.2. Que hem après

Hem aprofundit una poc més en l'ús de **Bootstrap** i hem descobert noves funcionalitats que ens han ajudat a millorar el disseny de les aplicacions i productivitat.

Cada membre de l'equip ha implementat diferents solucions i millores, com per exemple:

- Utilització de **placeholders** (*skeleton loaders*) per fer més dinàmica i fluida la càrrega de dades en algunes parts de les aplicacions.
- Implementació de **cards** per organitzar la informació de manera més clara i visual.
- Creació de taules, formularis i panells d'administració (**backoffice**) per facilitar la gestió de continguts i dades.
- Adaptació del disseny a diferents dispositius mitjançant el sistema de **grid responsive** de Bootstrap.
- Millora de l'experiència d'usuari a través de components interactius com ara **modals**, alertes i sistemes de navegació.
- Aprofundiment i millor aplicació del **SEO**.

## II.3. Que hem revisat d'usabilitat?

S'ha revisat aspectes relacionats amb la navegació, el disseny visual, l'adaptació responsive, la coherència entre pàgines, la internacionalització dels continguts, l'accessibilitat i el correcte funcionament dels enllaços i formularis.

L'ús de React ens ha permès expandir i millorar la usabilitat de l'aplicació, ja que la seua arquitectura basada en components reutilitzables ha facilitat:

- La correcció centralitzada d'errors de disseny.
- La unificació de criteris visuals entre pàgines.
- La implementació d'un comportament responsive més consistent.
- Una gestió més eficient de la navegació i la interacció amb l'usuari.
- El manteniment de l'aplicació i millores escalables en totes les seccions del projecte.

## II.4. No implementació usabilitat i ús de components

Dels nostres apartats hi han hagut varies coses que al final no hem pogut acabar d'implementar:

### II.4.a Stock
El stock no ha sigut implementat. Va ser proposat la seva implementació moltes vegades però el encarregat de dissenyar l'API va donar a entendre que no era una cosa necessària. Per implementar stock només necessitaríem un camp numèric anomenat `stock` en l'API de productes, implementar l'edició i poder afegir-lo en el BackOffice de Selectio, a més de restar-li al stock quan un producte és comprat.

### II.4.b  Filtres
La majoria dels filtres del BackOffice de Selectio no s'han pogut implementar, degut a que quan obtenim els elements (per exemple els productes) no obtenim tots — solament n'obtenim 10 degut a la paginació que es fa des de l'API de Laravel. Vam parlar amb el responsable de l'API i ens va comentar que ell posaria per a cada un un sistema de paginació des de l'API de Laravel i després nosaltres ho usaríem, però no va donar temps.

### II.4.c Checkbox en les taules
Simplement vam parlar amb David Crespo i vam decidir que solament fora estètic per falta de temps.

### II.4.d Idioma dels elements
La implementació de les traduccions en Selectio no es pot donar, ja que la traducció ha sigut implementada en l'últim moment i no es va pensar l'API per oferir diferents camps en diferents idiomes. Per poder implementar traducció en els productes hauríem de fer l'API amb els diversos camps i diversos idiomes, després comparar quin idioma està triat en la pàgina i a partir d'eixe idioma agafar de l'API els camps corresponents.