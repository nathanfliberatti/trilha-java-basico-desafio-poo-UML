classDiagram
    class ReprodutorMusical {
        +void tocar()
        +void pausar()
        +void selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +void ligar(numero: String)
        +void atender()
        +void iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +void exibirPagina(url: String)
        +void adicionarNovaAba()
        +void atualizarPagina()
    }

    interface ReprodutorMusical
    interface AparelhoTelefonico
    interface NavegadorInternet

    class iphone {
        tocar()
        pausar()
        selecionarMusica()
        ligar()
        atender()
        iniciarCorreioVoz()
        exibirPagina()
        adicionarNovaAba()
        atualizarPagina()
    }

    iphone --> ReprodutorMusical
    iphone --> AparelhoTelefonico
    iphone --> NavegadorInternet