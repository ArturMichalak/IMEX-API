> # IMEX-API
  
  
### Wzory zapytań

GET Header

* Lista objektów: kierowcówców **{drivers}**, zamówień **{orders}**, ciężarówek **{trucks}** lub tras **{routes}**.  
`https://example.com/{objekty}`  

* Lista zależna od informacji z działaniami **{equals}**, **{in}**, **{less-than}** i **{greater-than}** określonymi na zbiorach.  
`https://example.com/{objekty}/that-have-{własność}-{działanie}-{wartość}`

* Lista zależna od kilku informacji ze wzorca powyżej połączonymi słowami wykluczających **{and}** lub sumujących **{or}**.  
`https://example.com/{objekty}/that-have-{informacja}-{and/or}-{informacja}`

POST Header

* Nowy objekt: kierowca **{driver}**, zamówienie **{order}**, ciężarówka **{truck}** lub trasa **{route}**.  
`https://example.com/{objekt}`

GET/PUT Header

* Pierwszy objekt odnaleziony po informacji.  
`https://example.com/{objekt}/that-have-{własność}-{działanie}-{wartość}`

* Pierwszy odnaleziony po kilku informacjach.  
`https://example.com/{objekt}/that-have-{that-have}-{and/or}-{that-have}`
