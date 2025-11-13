# RESTAURANTE
Repositório destinado ao projeto de restaurante em BH. 

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cardápio Completo - Restaurante</title>

    <style>
        /* ======== ESTILOS GERAIS ======== */
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
                        url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092?auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
        }

        /* ======== TÍTULOS ======== */
        h1 {
            margin-top: 40px;
            font-size: 2.2em;
            color: #ffdd57;
            text-shadow: 2px 2px 5px #000;
        }

        h2 {
            margin-top: 20px;
            color: #ffd580;
        }

        /* ======== LISTAS E IMAGENS ======== */
        ul {
            list-style: none;
            padding: 0;
        }

        li {
            margin-top: 30px;
        }

        img {
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.4);
        }

        /* ======== TEXTOS ======== */
        figcaption {
            font-size: 1em;
            color: #f5f5f5;
            margin: 5px 0;
        }

        /* ======== FORMULÁRIOS E BOTÕES ======== */
        select, button {
            margin-top: 15px;
            padding: 10px 15px;
            border-radius: 5px;
            border: none;
            font-size: 1em;
        }

        button {
            background-color: #ffb347;
            color: #fff;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        button:hover {
            background-color: #ff9234;
        }

        form, p {
            margin-top: 20px;
        }

        /* ======== SEÇÃO DE SOBREMESAS ======== */
        section.sobremesas {
            margin-top: 80px;
            padding: 50px 0;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.6)),
                        url('https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-attachment: fixed;
            background-position: center;
        }

        section.sobremesas h1 {
            color: #ffcc99;
        }

        section.sobremesas h2 {
            color: #ffe0b3;
        }

        section.sobremesas figcaption {
            color: #fffaf5;
        }

        section.sobremesas button {
            background-color: #ffb6b9;
        }

        section.sobremesas button:hover {
            background-color: #ff9aa2;
        }

        /* ======== RESPONSIVIDADE ======== */
        @media (max-width: 600px) {
            img {
                width: 90%;
            }

            h1 {
                font-size: 1.6em;
            }

            h2 {
                font-size: 1.2em;
            }
        }
    </style>
</head>

<body>
    <h1>BEM-VINDO À NOSSA REDE DE RESTAURANTES</h1>
    <h5>Localização: Bairro Floresta, Belo Horizonte, MG</h5>

    <h2>Confira nosso cardápio disponível:</h2>

    <ul>
        <li><h3>Prato 1: Lasanha à Bolonhesa</h3></li>
        <img src="https://www.anamariareceitas.com.br/wp-content/uploads/2022/10/Lasanha-a-bolonhesa.jpg" alt="Lasanha a Bolonhesa" width="300">
        <figcaption>Deliciosa lasanha com molho e queijo gratinado.</figcaption>
        <figcaption>Preço (R$): 25,00</figcaption>

        <li><h3>Prato 2: Frango grelhado</h3></li>
        <img src="https://st1.uvnimg.com/a6/6a/ed8ca091475d8bb5af9d0192e6a8/frango-grelhado-prato-0622-1400x800.jpg" alt="Frango grelhado" width="300">
        <figcaption>Frango suculento grelhado com arroz, salada e ervas finas.</figcaption>
        <figcaption>Preço (R$): 22,00</figcaption>

        <form>
            <label for="prato">Escolha um dos pratos:</label>
            <select id="prato" name="prato" required>
                <option value="">-- Selecione um Produto --</option>
                <option value="prato1">LASANHA À BOLONHESA</option>
                <option value="prato2">FRANGO GRELHADO</option>
            </select>
        </form>
    </ul>

    <!-- ======== SEÇÃO DE SOBREMESAS ======== -->
    <section class="sobremesas">
        <h1>SOBREMESAS</h1>
        <h5>Localização: Bairro Floresta, Belo Horizonte, MG</h5>
        <h2>Confira nosso cardápio de sobremesas disponível:</h2>

        <ul>
            <li><h3>Sobremesa 1: Pudim</h3></li>
            <img src="https://s2.glbimg.com/Nf-KP945kuUD7bW-n_gVKnwVRHc=/1200x/smart/filters:cover():strip_icc()/s.glbimg.com/po/rc/media/2015/09/18/20_25_50_851_pudim.jpg" alt="Pudim" width="300">
            <figcaption>Delicioso pudim caseiro com calda de caramelo.</figcaption>
            <figcaption>Preço (R$): 10,00</figcaption>

            <li><h3>Sobremesa 2: Mousse de Chocolate</h3></li>
            <img src="https://images.pexels.com/photos/3026810/pexels-photo-3026810.jpeg?cs=srgb&dl=pexels-ella-olsson-3026810.jpg&fm=jpg" alt="Mousse de Chocolate" width="300">
            <figcaption>Mousse cremoso feito com chocolate meio amargo.</figcaption>
            <figcaption>Preço (R$): 12,00</figcaption>

            <form>
                <label for="sobremesa">Escolha uma das sobremesas:</label>
                <select id="sobremesa" name="sobremesa" required>
                    <option value="">-- Selecione uma Sobremesa --</option>
                    <option value="sobremesa1">PUDIM</option>
                    <option value="sobremesa2">MOUSSE DE CHOCOLATE</option>
                </select>
            </form>

            <p><button>Ir para pagamento</button></p>
        </ul>
    </section>
</body>
</html>
