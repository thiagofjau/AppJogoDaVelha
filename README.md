# ❌ Jogo da Velha — .NET MAUI ⭕

![.NET MAUI](https://img.shields.io/badge/.NET%20MAUI-512BD4?style=for-the-badge&logo=.dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![XAML](https://img.shields.io/badge/XAML-0C54C1?style=for-the-badge&logo=visualstudio&logoColor=white)

Este é um aplicativo móvel multiplataforma de **Jogo da Velha** desenvolvido como parte das atividades acadêmicas de **Programação para Dispositivos Móveis II** na **FATEC Jaú**. O projeto explora a criação de interfaces declarativas, manipulação dinâmica de componentes em runtime e lógica de matrizes.

---

## 📱 Funcionamento do App

O projeto implementa a lógica clássica do jogo em um tabuleiro de 3x3 com as seguintes características:
* [cite_start]**Alternância de Turnos:** O sistema gerencia automaticamente a vez atual, alternando entre as peças **"X"** e **"O"** a cada clique válido[cite: 4, 25].
* [cite_start]**Mapeamento Dinâmico:** Ao clicar em qualquer quadrante, o app identifica o componente visual e captura suas coordenadas lógicas (`Grid.GetRow` e `Grid.GetColumn`)[cite: 7, 8, 28, 29].
* [cite_start]**Matriz de Estado:** As jogadas são espelhadas em tempo real dentro de uma matriz bidimensional (`string[,]`) no backend para centralizar a persistência do estado do tabuleiro[cite: 6, 9, 27, 30].

---

## 🧠 Conteúdos Aprendidos & Aplicados

### 🎨 Interface Visual (XAML)
* [cite_start]**Grid Dinâmico:** Estruturação da tela usando `<Grid>` com proporções fluidas (`*`) para garantir que o tabuleiro se adapte a qualquer tamanho de tela de smartphone[cite: 19].
* [cite_start]**Estilização com Resources:** Criação de um `<Style>` implícito para centralizar as propriedades dos botões (como `CornerRadius`, `FontSize` e `BackgroundColor`), eliminando redundância de código[cite: 18].
* [cite_start]**Gradientes:** Aplicação de um fundo moderno utilizando `<LinearGradientBrush>`[cite: 18].

### ⚙️ Lógica de Backend (C#)
* [cite_start]**Manipulação Genérica de Eventos:** Uso de um único método `Button_Clicked` para escutar múltiplos botões, identificando quem disparou o evento via técnicas de *Casting* com o parâmetro `sender`[cite: 3, 24].
* [cite_start]**Manipulação de Matrizes:** Uso prático de arrays bidimensionais (`GetLength`, iterações aninhadas) para rastreamento e depuração no console via `Debug.WriteLine`[cite: 6, 10, 11, 27, 31, 32].
* [cite_start]**Ciclo de Vida e Dimensionamento:** Ajuste programático do tamanho inicial da janela (`w.Width` e `w.Height`) na inicialização do app para simular perfeitamente a proporção de um celular em ambientes desktop[cite: 14, 15].

---

## 🛠️ Como Compilar e Executar

Para rodar este projeto localmente, você precisará do **Visual Studio** instalado com a carga de trabalho de desenvolvimento **.NET MAUI** configurada.

Este projeto contribuiu para o aprendizagem em manipulação de eventos, lógica de jogos,  estruturas de dados, gerenciamento de estado e construção de interfaces com interação em .NET MAUI. 



1. Clone o repositório:
   ```bash
   git clone [https://github.com/thiagofjau/AppJogoDaVelha.git](https://github.com/thiagofjau/AppJogoDaVelha.git)
