# DiceRoller

Esse projeto foi criado durante o curso Developing Android Apps with Koltin, da Google, para representar a "rolagem" de um dado. 
Apesar de simples, usa bastante conceitos do Android Development, como View, ViewGroup, Layout, Activity, etc.

Ele funciona apertando um botão chamado "Roll". Ao apertar, o código escolherá uma imagem de maneira aleatória e mostrará ao usuário.

Lógica usada para fazer a escolha da imagem:
```kotlin
private fun rollDice() {
    val drawableResource = when (Random.nextInt(6) + 1) {
      1 -> R.drawable.dice_1
      2 -> R.drawable.dice_2
      3 -> R.drawable.dice_3
      4 -> R.drawable.dice_4
      5 -> R.drawable.dice_5
      else -> R.drawable.dice_6
    }
```

## Contribuição
O app foi criado e testado em um dispositivo físico, Redmi Note 9s, mas é disponível para qualquer um que queira contribuir.

Caso tenha alguma ideia de como melhorar o app, realize os seguintes passos:

1. Para contribuir, basta fazer um fork. 
(<https://github.com/arturbruno17/DiceRoller/fork>)

2. Crie uma branch para sua modificação
(`git checkout -b feature/fooBar`)

3. Faça o commit
(`git commit -am "Add some fooBar"`)

4. Push
(`git push origin feature/fooBar`)

5. Crie um novo *Pull Request*
