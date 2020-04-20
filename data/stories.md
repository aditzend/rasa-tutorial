## happy path , cuando el usuario coopera

* hola
  - utter_saludar
  - utter_preguntar_nombre
* decir_nombre{"nombre":"Human"}
  - utter_confirmar_nombre

## cuando el usuario no coopera

* hola
  - utter_saludar
  - utter_preguntar_nombre
* despedida
  - utter_despedir
