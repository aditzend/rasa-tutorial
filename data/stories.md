## happy path

- bienvenida
  - utter_greet
- mood_great
  - utter_happy

## sad path 1

- bienvenida
  - utter_greet
- mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
- affirm
  - utter_happy

## sad path 2

- bienvenida
  - utter_greet
- mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
- deny
  - utter_goodbye

## say goodbye

- despedida
  - utter_goodbye

## bot challenge

- bot_challenge
  - utter_iamabot
