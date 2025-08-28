# Projeto Avatar com Jetpack Compose

Este projeto Android desenvolvido em **Kotlin** utiliza **Jetpack Compose** para criar uma interface moderna, incluindo a exibição de um avatar personalizado (arquivo `avatar.xml`) com recursos visuais como formatação circular, espaçamento e organização em `Composable Functions`.

## 🎯 Objetivo

Demonstrar a utilização de um recurso vetorial (`avatar.xml`) implementado em uma interface com **Jetpack Compose**, incluindo o uso de componentes como:

- `Image()` para exibir o avatar
- `CardMensagem()` para montar a visualização
- `Scaffold`, `Row`, `Column` e `Text`
- Estilização com `Modifier`, `clip()`, `padding()`, entre outros

## 📱 Telas/Componentes

### 🧩 CardMensagem
Exibe o avatar com nome e conteúdo da mensagem:

```kotlin
Image(
    painter = painterResource(id = R.drawable.avatar),
    contentDescription = "Foto do contato",
    modifier = Modifier
        .size(52.dp)
        .clip(CircleShape)
)

🖼️ avatar.xml

- Recurso vetorial localizado em res/drawable/avatar.xml, utilizado como imagem de perfil.

🔧 Tecnologias utilizadas

- Kotlin
- Jetpack Compose
- Android Studio
- Vector Drawable

👨‍💻 Integrantes do Grupo

- Gustavo Santos - RM 551775
- Felipe Tomé - RM 98775

📸 Preview do Avatar

Você pode visualizar o avatar isoladamente através da função @Preview:

@Preview(showBackground = true)
@Composable
fun PreviewAvatar() {
    JetpackComposeTheme {
        Image(
            painter = painterResource(id = R.drawable.avatar),
            contentDescription = "Avatar",
            modifier = Modifier
                .size(64.dp)
                .clip(CircleShape)
        )
    }
}

📝 Licença

Este projeto é apenas para fins educacionais.