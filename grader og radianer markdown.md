# Grader og radianer

Her ser vi på den matematiske sammenhengen mellom vinkelmålene grader og radianer.  
Vi lager funksjoner i python for å gjøre om mellom dem.

Definisjon av en radian:
Radian er et vinkelmål, definert ved buelengde delt på radius.

Se for deg en sirkel som deles inn i sektorer.
Én radian er da en sektor hvor buelengden _b_ er like lang som radiusen _r_.

_b_ = _r_

Det er plass til $ 2 \pi $ antall radianer i en sirkel.


## Fra grader til radianer

Forholdet mellom grader og radianer er:

$ 360 \unicode{xB0} = 2 \pi $

Vi kan dermed gjøre om fra grader til radianer denne måten:

$ radianer = \frac{grader}{180 \unicode{xB0}} \cdot \pi $

_Eksempel:_

Her regner vi om $ 45 \unicode{xB0} $ til radianer:

$ \frac{45 \unicode{xB0}}{180 \unicode{xB0}} \cdot \pi = 0,785 $

45 grader tilsvarer altså 0,785 radianer.

I python:


```python
pi = 3.14

def grader_til_radianer(grader):
    radianer = (grader / 180) * pi
    
    return radianer

print(grader_til_radianer(45))
print(grader_til_radianer(67))
print(grader_til_radianer(180))
```

    0.785
    1.168777777777778
    3.14



## Fra radianer til grader

Vi vet at:

$ radianer = \frac{grader}{180 \unicode{xB0}} \cdot \pi $

Ved hjelp av litt algebra kan vi skrive om til:

$ grader = \frac{radianer}{\pi} \cdot 180 \unicode{xB0} $

I python kan vi dermed lage denne funksjonen:


```python
pi = 3.14

def radianer_til_grader(radianer):
    grader = (radianer / pi) * 180
    
    return grader

print(radianer_til_grader(pi/2))
print(radianer_til_grader(pi))
print(radianer_til_grader(2*pi))
```

    90.0
    180.0
    360.0



## Se også:

 - https://no.wikipedia.org/wiki/Radian
 
