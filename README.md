> # IMEX-API
  
  
### Wzory zapytań

GET Header

* Lista obiektów: kierowcówców **{drivers}**, zamówień **{orders}**, ciężarówek **{trucks}** lub tras **{routes}**.  
```
https://example.com/{obiekty}
```  

* Lista zależna od informacji z działaniami **{equals}**, **{in}**, **{less-than}** i **{greater-than}** określonymi na zbiorach.  
```
https://example.com/{obiekty}/that-have-{własność}-{działanie}-{wartość}
```

* Lista zależna od kilku informacji ze wzorca powyżej połączonymi słowami wykluczających **{and}** lub sumujących **{or}**.  
```
https://example.com/{obiekty}/that-have-{informacja}-{łącznik}-{informacja}
```

POST Header

* Nowy obiekt: kierowca **{driver}**, zamówienie **{order}**, ciężarówka **{truck}** lub trasa **{route}**.  
```
https://example.com/{obiekt}
```

GET/PUT Header

* Pierwszy obiekt odnaleziony po informacji.  
```
https://example.com/{obiekt}/that-have-{własność}-{działanie}-{wartość}
```

* Pierwszy odnaleziony po kilku informacjach.  
```
https://example.com/{obiekt}/that-have-{that-have}-{łącznik}-{that-have}
```
