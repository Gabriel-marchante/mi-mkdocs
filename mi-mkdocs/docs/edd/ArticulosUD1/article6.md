# Revisió de Sprint: Problemes Amb Tasques No Finalitzades

Durant la reunió de **revisió de sprint**, hem detectat diversos problemes amb algunes tasques que:

- No s'han completat a temps
- No s'han dut a terme correctament

Aquestes incidències poden haver-se derivat d'errors en la **planificació inicial del sprint**, on es van expressar preocupacions per part del **Scrum Master** sobre la càrrega de treball dels equips.

## Què ha passat?

Durant la reunió de planificació, el **Scrum Master** va advertir que alguns equips estaven sobrecarregats, fet que podria conduir a problemes de **productivitat** i **compliment dels terminis**.

No obstant això, el **Product Owner** va insistir en la necessitat d'acabar certes tasques ràpidament, degut a la **pressió del client**, que esperava veure aquests elements finalitzats de manera immediata.

### Causes Probables

- **Sobreassignació de tasques**: El fet que el Scrum Master ja alertés d'una sobrecàrrega de feina pot indicar que l'equip no tenia capacitat suficient per complir amb tots els **objectius del sprint**.
  
- **Pressió del client**: L'urgència per part del client podria haver forçat el **Product Owner** a incloure més tasques del que era raonable per a l'equip.

- **Manca de negociació**: Una falta de negociació efectiva entre el Product Owner i el Scrum Master pot haver portat a una planificació poc realista.

### Possibles Solucions

1. **Revisió de la càrrega de treball**: És essencial que el **Scrum Master** i el **Product Owner** treballin junts per garantir que la càrrega assignada a l'equip sigui realista.

2. **Establir prioritats clares**: El Product Owner ha d'assegurar-se que es prioritzen les tasques més importants, i que les tasques de menys urgència es poden reprogramar per a sprints futurs.

3. **Més comunicació amb el client**: Pot ser útil que el Product Owner negociï amb el client per ajustar les seves expectatives en funció del ritme de treball de l'equip.

---

### Exemples de problemes en el codi:

```python
# Aquest és un exemple d'un codi Python que no es va completar correctament:
def calcul_previsio(temps_total, tasques_completades):
    if tasques_completades == 0:
        return None  # Problema: No es gestiona el cas de zero tasques
    return temps_total / tasques_completades

# Solució: Afegir una condició per evitar la divisió per zero
def calcul_previsio(temps_total, tasques_completades):
    if tasques_completades == 0:
        return "No es pot calcular previsió, zero tasques completades"
    return temps_total / tasques_completades
```

---

## Taula de Comparativa Entre Sprints

| Sprint             | Tasques Assignades | Tasques Completes | Issues Detectats |
|--------------------|--------------------|-------------------|------------------|
| Sprint 1           | 20                 | 18                | 2                |
| Sprint 2           | 25                 | 19                | 6                |
| Sprint Actual      | 30                 | 20                | 10               |

---